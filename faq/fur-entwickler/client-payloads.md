# Client Payloads

GrieferGames sendet sogenannte Custom Plugin Messages (Client Payloads) über einen dedizierten Kanal an verbundene Clients. Diese Seite dokumentiert alle verfügbaren Payloads, ihr binäres Übertragungsformat und wie du sie in deinem Mod empfangen kannst.

## Übersicht

| Eigenschaft       | Wert                                            |
| ----------------- | ----------------------------------------------- |
| **Kanal**         | `griefergames:main`                             |
| **Richtung**      | Server → Client (unidirektional)                |
| **Registrierung** | Keine client-seitige Registrierung erforderlich |

{% hint style="info" %}
Du musst **kein** Registrierungs- oder Handshake-Paket an den Server senden. Der Server schickt die Payloads eigenständig an jeden verbundenen Client.
{% endhint %}

## Verfügbarkeit

| Umgebung  | Wo werden Payloads gesendet?                              |
| --------- | --------------------------------------------------------- |
| **1.8**   | Auf allen Servern **außer** der Lobby und dem Portalraum  |
| **Cloud** | Alle Server auf denen die Verwendung von Geld möglich ist |

## Übertragungsformat

Alle Payloads teilen dieselbe äußere Struktur auf dem `griefergames:main`-Channel:

```
┌──────────────────────────────────┐
│  id        UTF (Java DataOutput) │  ← Payload-Identifikator
│  <body>    payload-spezifische   │      ← Felder je nach Payload (siehe unten)
│            Daten                 │
└──────────────────────────────────┘
```

Der **UTF-String** wird im Java-[`DataOutputStream.writeUTF`](https://docs.oracle.com/javase/8/docs/api/java/io/DataOutputStream.html#writeUTF-java.lang.String-)-Format kodiert:

* 2 Bytes Big-Endian Unsigned Short → Länge der folgenden UTF-8-Byte-Sequenz
* N Bytes → String-Inhalt in modifiziertem UTF-8

Alle nachfolgenden numerischen Felder folgen der Standard-Big-Endian-Kodierung von [DataOutputStream](https://docs.oracle.com/javase/8/docs/api/java/io/DataOutputStream.html).

## Verfügbare Payloads

### `accountbalance`

Wird an den Client gesendet, sobald sich das Bargeld des Spielers ändert, sowie einmalig beim Betreten eines Servers.

| Feld      | Typ                                     | Beschreibung                                                   |
| --------- | --------------------------------------- | -------------------------------------------------------------- |
| `id`      | UTF                                     | `"accountbalance"`                                             |
| `balance` | `double` (8 Bytes, Big-Endian IEEE 754) | Aktuelles Guthaben des Spielers, auf 2 Dezimalstellen gerundet |

**Beispiel-Hex-Aufschlüsselung (Guthaben = `1234.56`):**

```
00 0D 61 63 63 6F 75 6E 74 62 61 6C 61 6E 63 65   ← UTF: 2-Byte-Länge (13) + "accountbalance"
40 93 4A 3D 70 A3 D7 0A                           ← double: 1234.56
```

## Payloads empfangen — Code-Beispiele

{% tabs %}
{% tab title="Fabric (>= 1.20.5)" %}
```java
import net.fabricmc.api.ClientModInitializer;
import net.fabricmc.fabric.api.client.networking.v1.ClientPlayNetworking;
import net.fabricmc.fabric.api.networking.v1.PayloadTypeRegistry;
import net.minecraft.network.PacketByteBuf;
import net.minecraft.network.codec.PacketCodec;
import net.minecraft.network.packet.CustomPayload;
import net.minecraft.util.Identifier;

import java.io.ByteArrayInputStream;
import java.io.DataInputStream;

public class MeinModClient implements ClientModInitializer {

    public static final Identifier CHANNEL_ID = Identifier.of("griefergames", "main");

    public record GrieferGamesPayload(byte[] data) implements CustomPayload {

        public static final CustomPayload.Id<GrieferGamesPayload> ID = new CustomPayload.Id<>(CHANNEL_ID);

        public static final PacketCodec<PacketByteBuf, GrieferGamesPayload> CODEC = PacketCodec.of(
                (payload, buf) -> buf.writeBytes(payload.data()),
                buf -> {
                    byte[] bytes = new byte[buf.readableBytes()];
                    buf.readBytes(bytes);
                    return new GrieferGamesPayload(bytes);
                }
        );

        @Override
        public Id<? extends CustomPayload> getId() {
            return ID;
        }
    }

    @Override
    public void onInitializeClient() {
        PayloadTypeRegistry.playS2C().register(GrieferGamesPayload.ID, GrieferGamesPayload.CODEC);
        ClientPlayNetworking.registerGlobalReceiver(GrieferGamesPayload.ID, (payload, context) -> {
            try (DataInputStream in = new DataInputStream(new ByteArrayInputStream(payload.data()))) {
                String id = in.readUTF();

                switch (id) {
                    case "accountbalance": {
                        double balance = in.readDouble();

                        // Guthaben verarbeiten
                        context.client().execute(() -> MeinMod.onMoneyUpdate(balance));
                        break;
                    }

                    default:
                        // Unbekannte ID ignorieren
                        // Neue Payloads können jederzeit hinzukommen
                        break;
                }

            } catch (Exception e) {
                e.printStackTrace();
            }
        });
    }
}
```
{% endtab %}

{% tab title="Forge (<= 1.12.2)" %}
```java
import io.netty.buffer.ByteBuf;
import net.minecraft.client.Minecraft;
import net.minecraftforge.fml.common.Mod;
import net.minecraftforge.fml.common.event.FMLInitializationEvent;
import net.minecraftforge.fml.common.eventhandler.SubscribeEvent;
import net.minecraftforge.fml.common.network.FMLEventChannel;
import net.minecraftforge.fml.common.network.FMLNetworkEvent;
import net.minecraftforge.fml.common.network.NetworkRegistry;

import java.io.ByteArrayInputStream;
import java.io.DataInputStream;

@Mod(modid = "meinmod", name = "MeinMod", version = "1.0")
public class MeinMod {

   private static final String CHANNEL = "griefergames:main";

   @Mod.EventHandler
   public void init(FMLInitializationEvent event) {
      // Kanal registrieren und diese Klasse als Listener anmelden
      FMLEventChannel channel = NetworkRegistry.INSTANCE.newEventDrivenChannel(CHANNEL);
      channel.register(this);
   }

   @SubscribeEvent
   public void onCustomPacket(FMLNetworkEvent.ClientCustomPacketEvent event) {
      ByteBuf buf = event.getPacket().payload();
      byte[] data = new byte[buf.readableBytes()];
      buf.readBytes(data);

      try (DataInputStream in = new DataInputStream(new ByteArrayInputStream(data))) {
         String id = in.readUTF();

         switch (id) {
            case "accountbalance": {
               double balance = in.readDouble();

               // Handler läuft im Netty-Thread -> auf den Client-Thread wechseln
               Minecraft.getMinecraft().addScheduledTask(() -> onMoneyUpdate(balance));
               break;
            }

            default:
               // Unbekannte ID ignorieren
               // Neue Payloads können jederzeit hinzukommen
               break;
         }

      } catch (Exception e) {
         e.printStackTrace();
      }
   }
}
```
{% endtab %}

{% tab title="LabyMod" %}
```java
import net.labymod.api.client.component.event.PluginMessageEvent;
import net.labymod.api.event.Subscribe;

import java.io.DataInputStream;
import java.io.ByteArrayInputStream;

public class MeinPayloadListener {

    @Subscribe
    public void onPluginMessage(PluginMessageEvent event) {
        if (!"griefergames:main".equals(event.getIdentifier())) return;

        byte[] data = event.getData();
        try (DataInputStream in = new DataInputStream(new ByteArrayInputStream(data))) {
            String id = in.readUTF();

            switch (id) {
                case "accountbalance": {
                    double balance = in.readDouble();

                    // Guthaben verarbeiten
                    MeinAddon.onMoneyUpdate(balance);
                    break;
                }
                default:
                    // Unbekannte ID ignorieren
                    // Neue Payloads können jederzeit hinzukommen
                    break;
            }
        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}
```

Den Listener im `AddonEntryPoint` registrieren:

```java
labyAPI().eventBus().registerListener(new MeinPayloadListener());
```
{% endtab %}

{% tab title="Vanilla / Protokoll-Ebene" %}
Das Payload kommt als clientbound **Plugin Message**-Packet auf dem Channel `griefergames:main` an. Den Datenbereich mit einem [DataInputStream](https://docs.oracle.com/javase/8/docs/api/java/io/DataInputStream.html) lesen, wie in den Beispielen oben gezeigt.

| Protokollversion | Packet-ID                              |
| ---------------- | -------------------------------------- |
| 1.8              | `0x3F`                                 |
| 1.21+            | `0x02` (Configuration) / `0x18` (Play) |
{% endtab %}
{% endtabs %}

## Zukunftssicherheit

Das Payload-System ist erweiterbar. Beim Empfang eines Payloads immer:

{% stepper %}
{% step %}
### Zuerst das `id`-Feld lesen.
{% endstep %}

{% step %}
### Per `switch`/`if` auf die ID reagieren und **unbekannte IDs ignorieren**.

Neue Payloads können jederzeit hinzukommen.
{% endstep %}

{% step %}
### Keine feste Gesamtlänge der Packetdaten annehmen.
{% endstep %}
{% endstepper %}

## Kurzübersicht

```
Kanal:  griefergames:main
Payloads:
  ┌──────────────────┬─────────────┬──────────────────────────────────────────────┐
  │ ID               │ Felder      │ Wann gesendet                                │
  ├──────────────────┼─────────────┼──────────────────────────────────────────────┤
  │ accountbalance   │ double      │ Beim Betreten eines Servers & bei jeder      │
  │                  │             │ Guthabenänderung                             │
  └──────────────────┴─────────────┴──────────────────────────────────────────────┘
```
