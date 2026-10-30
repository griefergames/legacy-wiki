---
description: Flags verändern das Spielverhalten auf dem jeweiligen Grundstück. Sie sind abhängig von Rechten und Grundstückseinstellungen.
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

# Grundstücks-Flags

## Feature-Flags

Diese Flags führen dazu, dass bestimmte Funktionen auf dem Grundstück freigeschaltet oder entfernt werden. Die meisten Flags erfordern nach ihrem Befehl einen Parameter, welcher die Funktion näher definiert.

| Funktion | Befehl | Parameter | Voraussetzung |
| --- | --- | --- | --- |
| Abschiedsnachricht setzen | `/p flag set farewell` | Text | Legende-Rang |
| Alias entfernen | `/p alias remove` | kein | Spieler-Rang |
| Alias setzen | `/p alias set` | Beliebiger Text | Spieler-Rang |
| Angreifen von Wölfen, Pferden und Katzen (de-)aktivieren | `/p flag set tamed-attack` | true / false | Spieler-Rang |
| Begrüßungsnachricht setzen | `/p flag set greeting` | Text | Legende-Rang |
| Benachrichtigung (de-)aktivieren: Spieler betritt das Grundstück | `/p flag set notify-enter` | true / false | Legende-Rang |
| Benachrichtigung (de-)aktivieren: Spieler verlässt das Grundstück | `/p flag set notify-leave` | true / false | Legende-Rang |
| Benutzung von Enderperlen durch Besucher (de-)aktivieren | `/p flag set enderpearl` | true / false | Spieler-Rang |
| Benutzung von Loren (de-)aktivieren | `/p flag set vehicle-use` | true / false | Spieler-Rang |
| Beschreibung entfernen | `/p description` | kein | Spieler-Rang |
| Beschreibung setzen | `/p description` | Beliebiger Text | Spieler-Rang |
| Bildung von Eis (de-)aktivieren | `/p flag set ice-form` | true / false | Spieler-Rang |
| Bildung von Schnee (de-)aktivieren | `/p flag set snow-form` | true / false | Spieler-Rang |
| Bossbar von Wither und Enderdrachen ausblenden | `/p flag set show-bossbar` | true / false | Spieler-Rang |
| Dorfbewohnerhandel (de-)aktivieren | `/p flag set villager-interact` | true / false | Spieler-Rang |
| Einsatz von Feuerwerk (de-)aktivieren | `/p flag set firework` | true / false | Spieler-Rang |
| Einsaugmodus der Unendlichen Lager zurücksetzen | `/storage clear` | kein | Spieler-Rang |
| Explosionen (de-)aktivieren | `/p flag set explosion` | true / false | Spieler-Rang |
| Fliegen (de-)aktivieren | `/p flag set allowfly` | true / false | Spieler-Rang |
| Forcefield (de-)aktivieren | `/p flag set forcefield` | true / false | Forcefield-Recht aus der Vote-/Supreme-Kiste |
| Interaktion mit Blöcken zulassen | `/p flag set use` | ID | Spieler-Rang |
| Interaktion mit Tieren (de-)aktivieren | `/p flag set animal-interact` | true / false | Spieler-Rang |
| Lagerterminal freigeben | `/p flag set unlimited-storageterminal-public` | true / false | Spieler-Rang |
| Musik setzen | `/p flag set music` | ID | Legende-Rang |
| Paintball-Gun-Funktion einschränken (nur Besitzer/Vertraute) | `/p flag set anti-gun` | true / false | Spieler-Rang |
| Portalgun-Funktion erlauben/verbieten | `/p flag set portal` | true / false | Spieler-Rang |
| PvE (de-)aktivieren | `/p flag set pve` | true / false | Spieler-Rang |
| PvP (de-)aktivieren | `/p flag set pvp` | true / false | Spieler-Rang |
| Schmelzen von Eis (de-)aktivieren | `/p flag set ice-melt` | true / false | Spieler-Rang |
| Schmelzen von Schnee (de-)aktivieren | `/p flag set snow-melt` | true / false | Spieler-Rang |
| Setzen und Nutzen von Home-Punkten durch Besucher (de-)aktivieren | `/p flag set allow-homes` | true / false | Spieler-Rang |
| Tageszeit (Helligkeit) auf dem Grundstück auf festen Wert setzen | `/p flag set time` | Zahl (0-24000) | Spieler-Rang |
| Teleportationsanfragen auf dem Grundstück (de-)aktivieren | `/p flag set allow-tpa` | true / false | Spieler-Rang |
| Titel beim Betreten setzen | `/p flag set enter-title` | Text | Spieler-Rang, eingelöstes Item |
| Titel beim Verlassen setzen | `/p flag set leave-title` | Text | Spieler-Rang, eingelöstes Item |
| Töten von Monstern (de-)aktivieren | `/p flag set hostile-attack` | true / false | Spieler-Rang |
| Töten von Tieren (de-)aktivieren | `/p flag set animal-attack` | true / false | Spieler-Rang |
| Unendliches Lager freigeben | `/p flag set unlimited-storage-public` | true / false | Spieler-Rang |
| Unsichtbarkeit auf dem Grundstück verbieten | `/p flag set anti-unsichtbarkeit` | true / false | Spieler-Rang |
| Untertitel beim Betreten setzen | `/p flag set enter-subtitle` | Text | Spieler-Rang, eingelöstes Item |
| Untertitel beim Verlassen setzen | `/p flag set leave-subtitle` | Text | Spieler-Rang, eingelöstes Item |
| Verkleiden (de-)aktivieren | `/p flag set disguise` | true / false | Spieler-Rang |
| Vertrauten das Bearbeiten von Showcase-Truhen und Vitrinen erlauben | `/p flag set trusted-showcase-edit` | true / false | Spieler-Rang |
| Wachstum von Gras (de-)aktivieren | `/p flag set grass-grow` | true / false | Spieler-Rang |
| Wachstum von Myzel (de-)aktivieren | `/p flag set mycel-grow` | true / false | Spieler-Rang |
| Wachstum von Ranken (de-)aktivieren | `/p flag set vine-grow` | true / false | Spieler-Rang |
| Wetter des Grundstücks auf „Regen“ oder „Normal“ umschalten | `/p flag set weather` | rain / clear | Spieler-Rang |
| Würfeln erlauben | `/p flag set dice` | true / false | Spieler-Rang |
| Zeigt eine Übersicht aktivierter Flags und bietet die Möglichkeit, diese per Klick zu entfernen. | `/removeflags` | kein | Spieler-Rang |

## Wetter auf dem Grundstück ändern

Spieler haben die Möglichkeit, das Wetter auf ihrem Grundstück mithilfe von Plot-Flags individuell anzupassen. Dies umfasst sonniges Wetter, Regen sowie das Erzeugen von Schneefall.

#### Wetter auf Sonne oder Regen stellen
Mit den folgenden Befehlen lässt sich das grundlegende Wetter auf dem Plot steuern:

* **Sonnenschein (Klar):** `/p flag set weather clear`
* **Regen:** `/p flag set weather rain`

###### Schnee auf dem Grundstück aktivieren
Minecraft erzeugt Schnee nur in kalten Biomen. Damit es auf dem Plot schneit, muss daher zuerst das Biom geändert und anschließend der Niederschlag aktiviert werden. 

Führe diese beiden Schritte nacheinander aus:

1. **Biom ändern:** z.B. `/p biome ICE_PLAINS`

{% hint style="info" %}
Damit die Biom-Änderung visuell sichtbar wird, musst du das Grundstück einmal verlassen und wieder betreten oder dich neu einloggen.
{% endhint %}
2. **Schneefall (Niederschlag) starten:** `/p flag set weather rain`


## Besonderheiten der „attack“-Flags

Die Grundstück-Flags `animal-attack`, `tamed-attack` und `hostile-attack` betreffen ausgewählte Entities, basierend auf der Kernmechanik von Minecraft zur Einstufung von Kreaturen. Bei Aktivierung können diese auch ohne aktivierte PvE-Flag angegriffen und getötet werden.

* Dorfbewohner werden als friedliche Kreatur gewertet und fallen unter die Flag `animal-attack`!
* Wölfe, Pferde und Katzen fallen unter die eigene Flag `tamed-attack`.
* Schleime, Lavaschleime, Tintenfische und Schneegolems gehören zu keiner dieser Kategorien und werden von den Flags nicht beeinflusst.

## „use“-Flag

Mit der **„use“-Flag** kann man anderen Spielern erlauben, bestimmte Blöcke auf dem eigenen Grundstück zu benutzen bzw. mit ihnen zu interagieren.

Die Flag wird mit folgendem Befehl gesetzt: `/p flag set use [Block-ID]`

Möchte man mehrere Blockarten freigeben, trennt man die IDs mit Kommas: `/p flag set use 1,2,3`

Bei mehr als drei IDs müssen zwischen den Zahlen und Kommas Buchstaben eingefügt werden: `/p flag set use 1,2,3,x,4,x,5`

{% hint style="danger" %}
**Die Verwendung von `use 0` ist nicht empfehlenswert!** Die ID `0` steht für Luft. Dadurch wird die Interaktion mit **allen Blöcken** freigegeben, wodurch Spieler auf alles auf dem Grundstück zugreifen können. Bitte nutzt daher die ID des Blockes, den ihr für alle freigeben möchtet.
{% endhint %}

Möchte man alle „use“-Flags deaktivieren, wird anstatt der IDs der Wert „false“ verwendet: `/p flag set use false`

### Wie finde ich die ID eines Blocks heraus?

* [Offizielles Minecraft-Wiki](https://minecraft-de.gamepedia.com/Numerische_Identifikation#Block-IDs)
* Google
* [ID-Liste](https://minecraft-ids.grahamedgecombe.com/) von Graham Edgecombe
* F3 + H (Tastenkombination in Minecraft) zeigt die ID hinter dem Namen des Items an

## „music“-Flag

Mit der „music“-Flag lassen sich auf dem Grundstück die verschiedenen Minecraft-eigenen Musikstücke wiedergeben. Hierfür werden die IDs der jeweiligen Schallplatten benötigt.

Der Befehl hierfür lautet `/p flag set music [ID]`.

<table><thead><tr><th align="center">Musikstück</th><th align="center">Befehl</th></tr></thead><tbody><tr><td align="center">13</td><td align="center"><code>/p flag set music 2256</code></td></tr><tr><td align="center">Cat</td><td align="center"><code>/p flag set music 2257</code></td></tr><tr><td align="center">Blocks</td><td align="center"><code>/p flag set music 2258</code></td></tr><tr><td align="center">Chirp</td><td align="center"><code>/p flag set music 2259</code></td></tr><tr><td align="center">Far</td><td align="center"><code>/p flag set music 2260</code></td></tr><tr><td align="center">Mall</td><td align="center"><code>/p flag set music 2261</code></td></tr><tr><td align="center">Mellohi</td><td align="center"><code>/p flag set music 2262</code></td></tr><tr><td align="center">Stal</td><td align="center"><code>/p flag set music 2263</code></td></tr><tr><td align="center">Strad</td><td align="center"><code>/p flag set music 2264</code></td></tr><tr><td align="center">Ward</td><td align="center"><code>/p flag set music 2265</code></td></tr><tr><td align="center">11</td><td align="center"><code>/p flag set music 2266</code></td></tr><tr><td align="center">Wait</td><td align="center"><code>/p flag set music 2267</code></td></tr></tbody></table>

Will man die gesetzte Musik auf dem Grundstück wieder deaktivieren, muss eine ID genutzt werden, welche keiner Schallplatte zugehörig ist (bspw. 9999).

Alternativ kann man den Befehl `/removeflags` zum Entfernen der Flag verwenden.

<details>

<summary>An diesem Artikel beteiligt</summary>

* [50U7R34P3R](https://profile.griefergames.live/minecraft/8e2ce0be-aa2c-46a7-a2dc-48f948743edf)

</details>
