---
description: Aufbau und Funktionen des Grundstück-Menüs
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

# Grundstück-Menü

Auf deinem Grundstück hast du die Möglichkeit, deine Besucher zu grüßen oder bestimmte Blöcke auf deinem Grundstück freizugeben. Auch kannst du dich vor Angriffen schützen, eine Kampfarena errichten oder entscheiden, ob das Gras auf deinem Grundstück wachsen darf oder du doch lieber einen Erdboden besitzt.

Hierfür stellen wir dir das Grundstücks-Menü vor, in welchem du viele verschiedene Einstellungen findest.

Das Menü rufst du auf deinem Grundstück mit `/plot`, `/p`, `/menü` oder `/m` auf.

![](../../.gitbook/assets/gdoc-606b18bbe470.png)

| Icon / Bezeichnung | Befehl | Funktion |
| --- | --- | --- |
| ![](../../.gitbook/assets/gdoc-ab566512d03f.png) |  | Grundstücksbefehle |
| <p><img src="../../.gitbook/assets/gdoc-6a860a016518.png" alt=""><br>Grundstückschat - /p chat</p> | `/p chat` | Hier hast du die Möglichkeit, auszuwählen, dass deine Chatnachrichten nur auf dem Grundstück zu lesen sind. |
| <p><img src="../../.gitbook/assets/gdoc-46a837fc6653.png" alt=""><br>Alias entfernen</p> | `/p alias remove` | Hier hast du die Möglichkeit, den Alias deines Grundstücks zu entfernen. |
| <p><img src="../../.gitbook/assets/gdoc-ba482ffb128c.png" alt=""><br>Beschreibung entfernen</p> | `/p description remove` | Entferne die Beschreibung deines Grundstücks. |
| <p><img src="../../.gitbook/assets/gdoc-895a8ad94197.png" alt=""><br>Rechteentzug</p> | `/p remove *` | Entferne alle Rechte, die du vergeben hast. |
| ![](../../.gitbook/assets/gdoc-2ca3ea09b4d0.png)Grundstücksinformation | `/p i` | Schaue, wo sich dein Grundstück befindet und welcher Alias aktuell gesetzt ist. |
| <p><img src="../../.gitbook/assets/gdoc-62622a44f9d0.png" alt=""><br>Einstellungen zurücksetzen</p> |  | Klicke, um alle Einstellungen auf den Standard zurückzusetzen. |

## Grundstücks-Flags

![](../../.gitbook/assets/gdoc-8521624f067c.png)

![](../../.gitbook/assets/gdoc-f64818bae6ce.png)

| Icon / Bezeichnung | Befehl | Funktion |
| --- | --- | --- |
| ![](../../.gitbook/assets/gdoc-575110f6db49.png) |  | Grundstücks-Flags |
| <p><img src="../../.gitbook/assets/gdoc-cbd3653990c1.png" alt=""><br>PvP</p> | <p><code>/p flag set pvp true</code><br><code>/p flag set pvp false</code></p> | Ist PvP aktiviert, könnt ihr euch auf dem Grundstück gegenseitig Schaden zufügen. |
| <p><img src="../../.gitbook/assets/gdoc-22a6487f33e9.png" alt=""><br>Animal-Attack</p> | <p><code>/p flag set animal-attack true</code><br><code>/p flag set animal-attack false</code></p> | Ist Animal-Attack aktiviert, so können Spieler auf dem Grundstück Tiere angreifen. |
| <p><img src="../../.gitbook/assets/gdoc-93ff39fe4684.png" alt=""><br>Hostile-Attack</p> | <p><code>/p flag set hostile-attack true</code><br><code>/p flag set hostile-attack false</code></p> | Ist Hostile-Attack aktiviert, so können Spieler auf dem Grundstück Monster angreifen. |
| <p><img src="../../.gitbook/assets/gdoc-f3d1b8dbc1e1.png" alt=""><br>Explosionen</p> | <p><code>/p flag set explosion true</code><br><code>/p flag set explosion false</code></p> | Sind Explosionen aktiviert, so kann TNT Schaden anrichten. |
| <p><img src="../../.gitbook/assets/gdoc-7860a77fcf6d.png" alt=""><br>Forcefield</p> | <p><code>/p flag set forcefield true</code><br><code>/p flag set forcefield false</code></p> | <p>Ist Forcefield aktiviert, stößt du Spieler zur Seite, die dir zu nahe kommen.</p><p><strong>Hinweis:</strong> Das <a href="https://items.griefergames.net/#Rechte_%7C_Forcefield_Flag">Forcefield-Flag-Item</a> aus der Supreme-Kiste wird benötigt.</p> |
| <p><img src="../../.gitbook/assets/gdoc-5429f7652fc2.png" alt=""><br>Dorfbewohnerhandel</p> | <p><code>/p flag set villager-interact true</code><br><code>/p flag set villager-interact false</code></p> | Erlaubt es Spielern, mit deinen Dorfbewohnern zu interagieren. |
| <p><img src="../../.gitbook/assets/gdoc-25122b07e087.png" alt=""><br>Loren-Nutzung</p> | <p><code>/p flag set vehicle-use true</code><br><code>/p flag set vehicle-use false</code></p> | Ist die Loren-Nutzung aktiviert, so dürfen Spieler deine Loren nutzen. |
| <p><img src="../../.gitbook/assets/gdoc-2ee54095942f.png" alt=""><br>Fliegen</p> | <p><code>/p flag set allowfly true</code><br><code>/p flag set allowfly false</code></p> | <p>Ist Fliegen aktiviert, so dürfen Spieler auf deinem Grundstück fliegen.</p><p><strong>Hinweis:</strong> <a href="https://items.griefergames.net/#Orb-Items_%7C_Flugtrank_">Fly-Trank</a>, Fly-Booster oder <a href="https://items.griefergames.net/#Plot-Fliegen">Plot-Fliegen</a> vorausgesetzt.</p> |
| <p><img src="../../.gitbook/assets/gdoc-f0e7619d1016.png" alt=""><br>Feuerwerke</p> | <p><code>/p flag set firework true</code><br><code>/p flag set firework false</code></p> | Erlaubt es Spielern, auf deinem Grundstück Feuerwerk abzuschießen. |
| <p><img src="../../.gitbook/assets/gdoc-a683fa8b56dc.png" alt=""><br>Disguise</p> | <p><code>/p flag set disguise true</code><br><code>/p flag set disguise false</code></p> | Diese Flag erlaubt bei Aktivierung, dass Spieler sich auf deinem Grundstück verkleiden. |
| <p><img src="../../.gitbook/assets/gdoc-43c40a6100c1.png" alt=""><br>Gras-Wachstum</p> | <p><code>/p flag set grass-grow true</code><br><code>/p flag set grass-grow false</code></p> | Ist Gras-Wachstum aktiviert, wächst Gras auf deinem Grundstück. |
| <p><img src="../../.gitbook/assets/gdoc-18255231a9c2.png" alt=""><br>Myzel-Wachstum</p> | <p><code>/p flag set mycel-grow true</code><br><code>/p flag set mycel-grow false</code></p> | Ist Myzel-Wachstum aktiviert, wächst Myzel auf deinem Grundstück. |
| <p><img src="../../.gitbook/assets/gdoc-c1b0ef55e883.png" alt=""><br>Ranken-Wachstum</p> | <p><code>/p flag set vine-grow true</code><br><code>/p flag set vine-grow false</code></p> | Ist Ranken-Wachstum aktiviert, wachsen Ranken auf deinem Grundstück. |
| <p><img src="../../.gitbook/assets/gdoc-80711692e23e.png" alt=""><br>Schnee-Formungen</p> | <p><code>/p flag set snow-form true</code><br><code>/p flag set snow-form false</code></p> | Ist diese Flag aktiviert, formt sich Schnee auf deinem Grundstück. |
| <p><img src="../../.gitbook/assets/gdoc-743df4ef2b65.png" alt=""><br>Schnee-Schmelzungen</p> | <p><code>/p flag set snow-melt true</code><br><code>/p flag set snow-melt false</code></p> | Ist diese Flag aktiviert, schmilzt der Schnee auf deinem Grundstück. |
| <p><img src="../../.gitbook/assets/gdoc-f642d90891e6.png" alt=""><br>Eis-Formungen</p> | <p><code>/p flag set ice-form true</code><br><code>/p flag set ice-form false</code></p> | Ist diese Flag aktiviert, formt sich Eis auf deinem Grundstück. |
| <p><img src="../../.gitbook/assets/gdoc-0f57803e6841.png" alt=""><br>Eis-Schmelzungen</p> | <p><code>/p flag set ice-melt true</code><br><code>/p flag set ice-melt false</code></p> | Ist diese Flag aktiviert, schmilzt das Eis auf deinem Grundstück. |
| <p><img src="../../.gitbook/assets/gdoc-0fce0a9a2223.png" alt=""><br>Tier-Interaktionen</p> | <p><code>/p flag set animal-interact true</code><br><code>/p flag set animal-interact false</code></p> | Erlaubt es Spielern, mit Tieren zu interagieren. |

## Use-Flag-Menü

![](../../.gitbook/assets/gdoc-335eb6a18b30.png)

| Icon / Bezeichnung | Befehl | Funktion |
| --- | --- | --- |
| ![](../../.gitbook/assets/gdoc-d6488d4b18e2.png) | `/p flag set use <ItemID>` | Use-Flag-Menü |

Mit dem Use-Flag-Menü hast du die Möglichkeit, gängige Blöcke für Spieler freizugeben.

Zur Auswahl stehen dir hier:

<table data-header-hidden><thead><tr><th></th><th width="108"></th><th></th><th width="159"></th><th></th></tr></thead><tbody><tr><td>Werkbänke</td><td>Öfen</td><td>Ambosse</td><td>Truhen</td><td>Braustände</td></tr><tr><td>Zaubertische</td><td>Spender</td><td>Endertruhen</td><td><a href="https://items.griefergames.net/#Mobiles_4-Gewinnt">4-Gewinnt</a></td><td>Spawner</td></tr><tr><td>Knöpfe</td><td>Hebel</td><td>Zauntore</td><td>Holzdruckplatte</td><td>Steindruckplatte</td></tr></tbody></table>

Ob eine Use-Flag gerade freigegeben ist, erkennst du daran, ob das Item leuchtet oder nicht.

Beispiel:

| ![](../../.gitbook/assets/gdoc-7606a331fe95.png)Werkbank nicht freigegeben | ![](../../.gitbook/assets/gdoc-c36b0735e0b8.png)Werkbank freigegeben |
| --- | --- |

## Weitere Menüpunkte

| Icon / Bezeichnung | Befehl | Funktion |
| --- | --- | --- |
| <p><img src="../../.gitbook/assets/gdoc-ab316dc56591.png" alt=""><br>Rand-Wand-Bodeneffekte</p> | <p><code>/rand</code><br><code>/wand</code><br><code>/boden</code></p> | <p>Hier findet ihr eine Auswahl an <a href="grundstuecke-veraendern.md">Rand-, Wand- und Bodeneffekten</a>.<br>Ihr könnt euren Grundstücksrand zum Beispiel in Quarzstufen oder auch Kohleblöcke verwandeln.</p><p><strong>Hinweis:</strong> Die Effekte sind <a href="../befehlsuebersicht/rang-befehle.md">rangabhängig</a>. Einige Effekte können auch nur in <a href="../features/das-case-opening.md#die-supreme-kiste">Supreme-Kisten</a> gewonnen werden.</p> |

Zusätzlich findest du in den Grundstücksbefehlen folgende Möglichkeiten:

| Icon / Bezeichnung | Befehl | Funktion |
| --- | --- | --- |
| <p><img src="../../.gitbook/assets/gdoc-0299136bce9c.png" alt=""><br>Aushöhlen</p> | `/aushöhlen` | Über diesen Befehl hast du die Möglichkeit, dein Grundstück von bestimmten Baumaterialien zu [befreien](grundstuecke-veraendern.md#aushoehlen). |
| <p><img src="../../.gitbook/assets/gdoc-17dc866f67f7.png" alt=""><br>Leucht-Effekt</p> | `/leuchten` | <p>Durch die Nutzung des Befehls werden auf der Straße an den Ecken deines Grundstücks Beacons platziert. Unter den Beacons befinden sich Diamantblöcke, sodass die Beacons aktiviert sind und einen Lichtstrahl nach oben erzeugen.</p><p><strong>Hinweis:</strong> Der Befehl muss vorher in der Supreme-Kiste gewonnen werden.</p> |
| <p><img src="../../.gitbook/assets/gdoc-475015aa1dca.png" alt=""><br>Grundstück kaufen</p> | `/p claim` | Hier kannst du per Mausklick ein freies Grundstück kaufen. |
| <p><img src="../../.gitbook/assets/gdoc-ad5d1d503f50.png" alt=""><br>Übersicht freier Grundstücke</p> |  | Diese Übersicht zeigt dir an, wie viele kostenlose Grundstücke du auf dem Citybuild zur Verfügung hast. |
