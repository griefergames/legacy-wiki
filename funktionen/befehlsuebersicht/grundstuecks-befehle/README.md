---
description: Befehle rund um dein Grundstück (Plot)
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

# Grundstücks-Befehle

Auf dieser Seite findest du alle Befehle rund um deine Grundstücke. `/p` ist dabei die Kurzform von `/plot`.

## Grundstücke erhalten

| Befehl | Funktion |
| --- | --- |
| `/p auto` | Erhalte ein zufällig gewähltes freies Grundstück |
| `/p claim` | Erhalte das freie Grundstück, auf welchem du dich aktuell befindest |
| `/checkplot` | [Grundstück eines inaktiven Spielers beantragen](../../grundstuecke/grundstuecke-inaktiver-spieler-beantragen.md) |

## Grundstücks-Teleport

| Befehl | Funktion |
| --- | --- |
| <p><code>/p h &lt;Zahl></code><br><code>/plot home &lt;Zahl></code><br><code>/p h &lt;ID></code></p> | <p>Teleportiere dich zu deinem Grundstück.</p><p>Beispiel: <code>/p h 2</code> bringt dich auf dein zweites Grundstück.</p> |
| <p><code>/p h &lt;Spielername> &lt;Zahl></code><br><code>/p h &lt;Alias></code></p> | Teleportiert dich zum Grundstück eines Mitspielers. |
| `/p middle` | Teleportiere dich zur Mitte des Grundstücks |
| <p><code>/p sethome</code><br><code>/p &lt;ID> sethome</code></p> | Versetze den Spawnpunkt des Grundstücks an deine aktuelle Position |

## Grundstück verwalten

| Befehl | Funktion |
| --- | --- |
| <p><code>/p i</code><br><code>/plot info</code></p> | Zeigt eine Übersicht mit [Informationen und Einstellungen des Grundstücks](grundstuecks-informationen.md) an |
| <p><code>/p</code><br><code>/plot</code><br><code>/m</code><br><code>/menu</code></p> | [Grundstücks-Menü](../../grundstuecke/grundstueck-menue.md) aufrufen |
| `/merge` | [Grundstücke verbinden](../../grundstuecke/grundstuecke-verbinden.md) |
| `/mergebug` | Fehler beim Verbinden an der aktuellen Position an das Team melden |
| `/p clear` | <p>Grundstück in den Ursprungszustand versetzen</p><p><strong>Achtung!</strong> Bei einem Merge werden die Grundstücke getrennt!</p> |
| <p><code>/p delete</code><br><code>/p reset</code></p> | Grundstück löschen und freigeben |

## Rechte verwalten

Natürlich könnt ihr auch gemeinschaftlich an Projekten arbeiten. Dazu könnt ihr anderen Spielern Rechte zuweisen oder unerwünschten Besuch fernhalten.

| Befehl | Funktion |
| --- | --- |
| `/p trust <Spielername>` | Der Spieler erhält volle Rechte auf deinem Grundstück und allem, was zum Grundstück gehört |
| `/p add <Spielername>` | Der Spieler verfügt nur dann über Rechte, wenn du auf dem Citybuild-Server online bist |
| `/p remove <Spielername>` | Du entziehst dem Spieler alle Rechte von deinem Grundstück |
| `/p deny <Spielername>` | Der Spieler wird von deinem Grundstück gebannt und kann dieses nicht mehr betreten |
| `/p undeny <Spielername>` | Der Spieler wird von deinem Grundstück entbannt und darf dein Grundstück wieder betreten. |
| `/p kick <Spielername>` | Der Spieler wird von deinem Grundstück geworfen, kann es aber direkt wieder betreten |

Setzt du statt eines Spielernamens ein `*` ein, so gilt dieser Befehl für alle Spieler.

{% hint style="info" %}
**Beispiele:**

* `/p trust AbgegrieftHD` – Abge darf sich auf deinem Grundstück austoben. Sonst niemand.
* `/p trust *` – Jeder Anwesende kann auf deinem Grundstück alles machen.
{% endhint %}

{% hint style="danger" %}
Rechte für alle Spieler zu vergeben ist nicht sonderlich ratsam und nur bedingt zu empfehlen.
{% endhint %}

## Weitere Grundstücks-Befehle

| Befehl | Funktion |
| --- | --- |
| `/setowner {Spielername}` | Starte eine Überschreibung deines Grundstücks an einen anderen Spieler |
| `/setowner confirm` | Bestätige die Überschreibung eines Grundstücks |
| `/setowner deny` | Lehne die Überschreibung eines Grundstückes ab |
| `/p description {Text}` | Füge deinem Grundstück eine Beschreibung hinzu |
| `/p description` | Entferne die Beschreibung des Grundstücks |
| `/p alias set {Text}` | <p>Gib dem Grundstück einen Namen (Alias)<br><br><strong>Achtung!</strong> Es können keine Namen von Spielern genutzt werden, welche bereits auf dem Server angemeldet sind/waren.</p> |
| <p><code>/p chat on</code><br><code>/p chat off</code></p> | <p>Schreibe im Grundstücks-Chat<br>Schreibe im Normalchat</p> |
| `/p flag set {Flag} {true/false/ID}` | [Grundstücks-Flag](grundstuecks-flags.md) setzen |
| `/p setorder {Zahl}` | Setzt das Grundstück an die ausgewählte Position deiner Grundstücksliste |
| `/bewertung` | Aktiviere die Bewertungsfunktion für dein Grundstück |
| `/bewerten` | Menü zur Grundstücks-Bewertung aufrufen |
| `/leuchten` | <p>Leuchtfeuer an den Grundstücksecken platzieren<br><em>(Recht kann im</em> <a href="../../features/das-case-opening.md"><em>CaseOpening</em></a> <em>gewonnen werden)</em></p> |
| `/rand` | Ändere den [Grundstücksrand](../../grundstuecke/grundstuecke-veraendern.md#rand) |
| `/wand` | Ändere die [Grundstückswände](../../grundstuecke/grundstuecke-veraendern.md#wand) |
| `/boden` | Ändere den [Grundstücksboden](../../grundstuecke/grundstuecke-veraendern.md#boden) |
| `/aushöhlen` | Öffne das Menü zum [Aushöhlen des Grundstücks](../../grundstuecke/grundstuecke-veraendern.md#aushohlen) |
| `/breakblock` | Baut einen geschützten Block (z. B. Barrieren, Endportalrahmen, Grundgestein und Spawner) auf deinem Grundstück ab. Der Block wird nach dem Anklicken abgebaut und geht verloren. |
