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

<table><thead><tr><th>Funktion</th><th>Befehl</th><th>Parameter</th><th>Voraussetzung</th></tr></thead><tbody><tr><td>Beschreibung setzen</td><td><code>/p description</code></td><td>Beliebiger Text</td><td>Spieler-Rang</td></tr><tr><td>Beschreibung entfernen</td><td><code>/p description</code></td><td>kein</td><td>Spieler-Rang</td></tr><tr><td>Alias setzen</td><td><code>/p alias set</code></td><td>Beliebiger Text</td><td>Spieler-Rang</td></tr><tr><td>Alias entfernen</td><td><code>/p alias remove</code></td><td>kein</td><td>Spieler-Rang</td></tr><tr><td><a href="grundstuecks-flags.md#use-flag">Interaktion mit Blöcken zulassen</a></td><td><code>/p flag set use</code></td><td>ID</td><td>Spieler-Rang</td></tr><tr><td>Explosionen (de-)aktivieren</td><td><code>/p flag set explosion</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>PvP (de-)aktivieren</td><td><code>/p flag set pvp</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>PvE (de-)aktivieren</td><td><code>/p flag set pve</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Wetter des Grundstücks auf „Regen“ oder „Normal“ umschalten</td><td><code>/p flag set weather</code></td><td>rain / clear</td><td>Spieler-Rang</td></tr><tr><td>Benutzung von Loren (de-)aktivieren</td><td><code>/p flag set vehicle-use</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Dorfbewohnerhandel (de-)aktivieren</td><td><code>/p flag set villager-interact</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Interaktion mit Tieren (de-)aktivieren</td><td><code>/p flag set animal-interact</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Töten von Tieren (de-)aktivieren</td><td><code>/p flag set animal-attack</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Töten von Monstern (de-)aktivieren</td><td><code>/p flag set hostile-attack</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Verkleiden (de-)aktivieren</td><td><code>/p flag set disguise</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Einsatz von Feuerwerk (de-)aktivieren</td><td><code>/p flag set firework</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Tageszeit (Helligkeit) auf dem Grundstück auf festen Wert setzen</td><td><code>/p flag set time</code></td><td>Zahl (0-24000)</td><td>Spieler-Rang</td></tr><tr><td>Wachstum von Ranken (de-)aktivieren</td><td><code>/p flag set vine-grow</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Wachstum von Gras (de-)aktivieren</td><td><code>/p flag set grass-grow</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Wachstum von Myzel (de-)aktivieren</td><td><code>/p flag set mycel-grow</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Bildung von Schnee (de-)aktivieren</td><td><code>/p flag set snow-form</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Bildung von Eis (de-)aktivieren</td><td><code>/p flag set ice-form</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Schmelzen von Schnee (de-)aktivieren</td><td><code>/p flag set snow-melt</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Schmelzen von Eis (de-)aktivieren</td><td><code>/p flag set ice-melt</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Portalgun-Funktion erlauben/verbieten</td><td><code>/p flag set portal</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Paintball-Gun-Funktion einschränken (nur Besitzer/Vertraute)</td><td><code>/p flag set anti-gun</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Fliegen (de-)aktivieren</td><td><code>/p flag set allowfly</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Würfeln erlauben</td><td><code>/p flag set dice</code></td><td>true / false</td><td></td></tr><tr><td><a href="grundstuecks-flags.md#music-flag">Musik setzen</a></td><td><code>/p flag set music</code></td><td>ID</td><td>Legende-Rang</td></tr><tr><td>Begrüßungsnachricht setzen</td><td><code>/p flag set greeting</code></td><td>Text</td><td>Legende-Rang</td></tr><tr><td>Abschiedsnachricht setzen</td><td><code>/p flag set farewell</code></td><td>Text</td><td>Legende-Rang</td></tr><tr><td>Benachrichtigung (de-)aktivieren:<br>Spieler betritt das Grundstück</td><td><code>/p flag set notify-enter</code></td><td>true / false</td><td>Legende-Rang</td></tr><tr><td>Benachrichtigung (de-)aktivieren:<br>Spieler verlässt das Grundstück</td><td><code>/p flag set notify-leave</code></td><td>true / false</td><td>Legende-Rang</td></tr><tr><td>Forcefield (de-)aktivieren</td><td><code>/p flag set forcefield</code></td><td>true / false</td><td>Forcefield-Recht aus der Vote-/Supreme-Kiste</td></tr><tr><td>Unendliches Lager freigeben</td><td><code>/p flag set unlimited-storage-public</code></td><td>true / false</td><td>Spieler-Rang</td></tr><tr><td>Einsaugmodus der Unendlichen Lager zurücksetzen</td><td><code>/storage clear</code></td><td>kein</td><td>Spieler-Rang</td></tr><tr><td>Zeigt eine Übersicht aktivierter Flags und bietet die Möglichkeit, diese per Klick zu entfernen.</td><td><code>/removeflags</code></td><td>kein</td><td>Spieler-Rang</td></tr></tbody></table>

## Besonderheiten der „attack“-Flags

Die Grundstück-Flags `animal-attack` und `hostile-attack` betreffen ausgewählte Entities, basierend auf der Kernmechanik von Minecraft zur Einstufung von Kreaturen. Bei Aktivierung können diese auch ohne aktivierte PvE-Flag angegriffen und getötet werden.

* Dorfbewohner werden als friedliche Kreatur gewertet und fallen unter die Flag `animal-attack`!
* Schleime, Lavaschleime, Tintenfische und Schneegolems gehören zu keiner der beiden Kategorien und werden von den Flags nicht beeinflusst.

## „use“-Flag

Mit der **„use“-Flag** kann man anderen Spielern erlauben, bestimmte Blöcke auf dem eigenen Grundstück zu benutzen bzw. mit ihnen zu interagieren.

Die Flag wird mit folgendem Befehl gesetzt: `/p flag set use [Block-ID]`

Möchte man mehrere Blockarten freigeben, trennt man die IDs mit Kommas: `/p flag set use 1,2,3`

Bei mehr als drei IDs müssen zwischen den Zahlen und Kommas Buchstaben eingefügt werden: `/p flag set use 1,2,3,x,4,x,5`

{% hint style="danger" %}
**Die Verwendung von `use 0` ist nicht empfehlenswert!** Die ID `0` steht für Luft. Dadurch wird die Interaktion mit **allen Blöcken** freigegeben, wodurch Spieler unter anderem auf Truhen, Öfen und andere interaktive Blöcke zugreifen können.
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
