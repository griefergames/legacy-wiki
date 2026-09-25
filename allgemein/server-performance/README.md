---
description: Limits, Whitelists und Remover
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: false
  metadata:
    visible: true
  tags:
    visible: true
  actions:
    visible: true
  anchors:
    visible: true
---

# 📉 Server-Performance

Auf dieser Seite erfährst du, wie die Leistung unserer Server gemessen wird, welche automatischen Schutzmaßnahmen (Remover, Slot-Beschränkungen, Whitelists) es gibt und warum Redstone auf deinem Grundstück eingeschränkt werden kann.

### Performancewerte

#### TPS

"Ticks pro Sekunde" ist die am häufigsten verwendete Einheit zur Angabe der Serverperformance.

Minecraft arbeitet mit einem eigenen Zeitsystem, welches mit sogenannten "Ticks" arbeitet. Ein Minecraft-Tag entspricht einer Zeitspanne von 24.000 Ticks. Auch der Server nutzt diese Angabe, um Änderungen in der Spielwelt zu verarbeiten. Das Bewegen von Entitäten, die Zeit zum Abbauen eines Blocks, Schaden erleiden/heilen und alle anderen Vorgänge werden bei jedem Tick ein wenig weiter geschoben.

Minecraft geht hierbei von einer optimalen Tickrate von 20 Ticks pro Sekunde aus (1 Tick = 50 ms / 0,05 Sekunden). Dabei kann der Server, gemessen an seiner Rechengeschwindigkeit, nur eine bestimmte Anzahl an "Rechenoperationen" vornehmen. Übersteigt die Anzahl an Verarbeitungen die Menge, so können diese nicht mehr in der vollen Geschwindigkeit ablaufen. Der Server "laggt" (engl. "lag behind" = hinterherhängen) und in einer Sekunde werden weniger Ticks abgearbeitet.

Die Performance des Servers fällt dann auf einen niedrigeren TPS-Wert. Es werden also weniger Ticks pro Sekunde ausgeführt. Aktionen, welche davon abhängig sind, benötigen entweder mehr Zeit zum Ausführen oder werden "zurückgesetzt", wenn zwischen dem Server und dem Spielclient unterschiedliche Zeitberechnungen stattfanden. Das tritt besonders oft beim Abbauen von Blöcken oder beim Bewegen von Spielfigur oder Kreaturen auf (sog. "Zurückbuggen").

#### CPU

Server arbeiten wie andere Informationssysteme mit einer CPU (Central Processing Unit), auch als Prozessor bezeichnet. Ein wesentliches Problem in der Performance ist, dass Minecraft als Anwendung lediglich einen Kern des Prozessors ansteuert und verwendet, was die maximale Rechenleistung der verwendeten Systeme stark einschränkt.

Selbst ein Multikernprozessor _(DualCore, QuadCore oder EightCore)_ auf einem Server bringt also keinen Vorteil, da der MainThread von Minecraft immer nur einen Kern ansteuern würde und die Leistung verloren ginge. Viele Prozesse können zudem bei Minecraft nicht asynchron abgearbeitet werden, da sie mit anderen in der Spielwelt zusammenhängen. Somit fällt auch eine Virtualisierung von mehreren Prozessoren auf einen aus. Der "virtualisierte" Einzelkern würde die Aufgaben an mehrere physische Kerne verteilen, was die Abarbeitung nicht nur "verzögert", sondern möglicherweise auch asynchronisiert und dadurch insgesamt zu mehr Problemen führt, als es löst.

Je mehr Aktionen also innerhalb der Spielwelt auftreten, desto stärker wird der Server hierdurch belastet. Je weiter die CPU-Auslastung ansteigt, desto mehr Aktionen muss der Server in kurzer Zeit "verarbeiten". Übersteigt die Menge der zu verarbeitenden Aktionen 5% der max. CPU-Last, so können 20 Ticks in einer Sekunde nicht mehr abgearbeitet werden (20 Ticks \* 5 % = 100 % Last pro Sekunde).

<figure class="wiki-illus"><img src="/img/wiki-illus/server-performance.webp" alt="Zu viele Entities, Hopper und Item Frames auf einem Grundstück kosten Leistung."><figcaption>Zu viele Entities, Hopper und Item Frames auf einem Grundstück kosten Leistung.</figcaption></figure>

Hat ein Server also mehr CPU-Last, muss er die Menge an Ticks reduzieren, damit er nicht überlastet wird. Wird die Menge an Ticks reduziert, fällt dies als schlechte Performance durch entsprechendes Fehlverhalten zwischen Server und Spiel-Client auf.

{% hint style="warning" %}
Fällt die Serverperformance unter entsprechende Schwellwerte, werden zur Stabilisierung verschiedene Vorgänge automatisch ausgeführt:

* Die Funktion von Redstone wird deaktiviert
* Der Lava- & Wasser-Fluss wird deaktiviert
* Auf Citybuild Nature werden alle Hühner gelöscht

Steigt die Performance wieder über den entsprechenden Schwellwert, wird die Maßnahme wieder außer Kraft gesetzt.
{% endhint %}

### Limits und Remover

#### Natürlicher Despawn

Minecraft löscht aus eigenem Antrieb Items und Kreaturen, um die benötigte Rechenleistung zu verringern.

* Kreaturen haben jeden Tick eine geringe Chance (0,125% = 1/800) zu despawnen, wenn sich für 600 Ticks (30 Sekunden) kein Spieler im Umkreis von 32 Blöcken befindet.
* Items werden nach 6000 Ticks (5 Minuten) entfernt, wenn sie in einem geladenen Chunk liegen und nicht von einem Spieler aufgenommen werden.

#### MobRemover

Der MobRemover entfernt alle 15 Minuten sämtliche Kreaturen in allen geladenen Chunks. Dorfbewohner können mit einem passenden [Token](https://items.griefergames.net/#Dorfbewohner-Token) hiervor gesichert werden.

#### ItemRemover

Der ItemRemover entfernt alle 20 Minuten frei schwebende Items in allen geladenen Chunks. Die Items gehen hierbei unwiederbringlich verloren, unabhängig davon, wie lange sie bereits in der Welt sind.

#### MoneyDrop-Stopp

Wird die [Join-Cap (Freie Serverslots)](./#join-cap-reservierte-slots-und-whitelists) des Servers überschritten, so werden keine [Moneydrops](https://items.griefergames.net/#10.000%24_10x-Money-Drop) aus den [Case-Opening-Kisten](../../funktionen/features/das-case-opening.md) mehr generiert. Die Kiste wird dem Spieler zurückerstattet.

### Join-Cap, Reservierte Slots und Whitelists

Zur Sicherung des Serverbetriebs ist es erforderlich, die Menge an Spielern auf den Servern zu beschränken.

Hierfür ist auf jedem Server eine Slot-Beschränkung („Cap“) aktiviert, welche sich in mehrere Stufen aufteilt:

* Die **„Join-Cap“,** welche der im Scoreboard angegebenen Zahl entspricht.
  * Alle Accounts (unabhängig ihrer Rechte) können den Server betreten.
* Die **„Soft-Cap“**, welche bis zu 150 Slots über dem Join-Cap liegt.
  * Accounts mit „Join-Rechten“ (konnten früher separat gebucht werden oder sind im Rang enthalten) können entsprechend ihrem Rang den Server betreten.
    * max. Slots + 50 = Premium, Ultra, Legende
    * max. Slots + 85 = Titan
    * max. Slots + 115 = Griefer
    * max. Slots + 150 = Supreme
* Die **„Whitelist“** wird automatisch vom System gesetzt, wenn der Server überfüllt ist **oder** von einem Teammitglied aktiviert, um die Serverstabilität zu sichern.
  * Nur entsprechend freigegebene Accounts (in der Regel hochrangige Teammitglieder) können den Server noch betreten.
* Der **„Wartungsmodus“**, welcher ausschließlich manuell durch einen Admin/Developer geschaltet wird, um einen Absturz des Servers wegen Überlast zu verhindern oder um Arbeiten an den Servern und der Software vorzunehmen.
  * Nur entsprechend freigegebene Accounts (in der Regel hochrangige Teammitglieder) können den Server noch betreten.

Das Schalten von Caps und Whitelists ist eine erforderliche Maßnahme, um die Stabilität der Server zu gewährleisten. Technische Belange des Servers (Ausfallprävention, Wartungen, etc.) fallen **nicht** unter die Leistungsbeschreibung der „Verfügbarkeit“.

{% hint style="warning" %}
Einzelne Citybuild-Server können von diesen Regelungen abweichen.
{% endhint %}

Die Slot-Beschränkungen von Servern können entsprechend der technischen Verfügbarkeit angepasst (verringert) werden. Eine Anhebung der Server-Slots bzw. individuelle Freischaltung vom Cap-/Whitelist-System ist aus Gründen der Performance nicht möglich.

### Redstone deaktiviert

Durch die Möglichkeit, die Server-Performance durch diverse Redstone-Konstruktionen zu beeinträchtigen, wurden Sicherheitsvorkehrungen an den Grundstücken vorgenommen. Durch diese Vorkehrung werden Grundstücke, die eine erhöhte Redstone-Aktivität vorweisen, automatisch von einem Plugin „eingeschränkt“, sodass die Redstone-Schaltung nicht mehr genutzt werden kann.

Ein Grundstück kann daher, wenn besonders viele, große oder schnelle Redstone-Schaltungen auf dem Grundstück verbaut sind, von der Benutzung von Redstone bis zum nächsten Server-Neustart (um 4 Uhr morgens) eingeschränkt werden.

Leider lässt sich diese Einschränkung des Grundstücks nicht manuell ändern.

**Das heißt:** Wenn diese Einschränkung ausgelöst wurde, musst du leider damit leben und solltest dir vorzugsweise noch einmal deine Konstruktionen näher anschauen und entscheiden, ob du diese etwas verkleinern kannst.

Aus Gründen der Sicherheit können wir natürlich nicht genau mitteilen, ab welchen Limits diese Einschränkungen aktiv werden.

<details>

<summary>An diesem Artikel beteiligt</summary>

* [50U7R34P3R](https://profile.griefergames.live/minecraft/8e2ce0be-aa2c-46a7-a2dc-48f948743edf)

</details>
