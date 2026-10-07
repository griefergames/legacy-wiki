---
description: Eigene NPCs auf deinem Grundstück aufstellen und einrichten
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

# Plot-NPCs

Mit einem **Plot-NPC** stellst du einen eigenen NPC auf dein Grundstück. Er kann z. B. als Orb-Händler, Auktionshaus oder Lotterie dienen, sodass du diese Menüs direkt auf deinem Grundstück öffnen kannst.

Aussehen, Name, Position und Funktion des NPCs legst du selbst fest.

{% hint style="danger" %}
Plot-NPCs werden gelöscht, wenn das Grundstück gelöscht oder zurückgesetzt wird. Das gilt auch, wenn [verbundene Grundstücke](grundstuecke-verbinden.md) wieder getrennt werden.
{% endhint %}

{% hint style="info" %}
Bei einer [Grundstücksverschiebung](grundstucke-verschieben-and-erweitern.md) durch das Team ziehen deine Plot-NPCs mit um. Art, Name, Funktion und Einstellungen bleiben dabei erhalten. Gib deine NPCs trotzdem wie beschrieben in deinem Antrag an.
{% endhint %}

## Plot-NPC erhalten

Für einen NPC brauchst du ein **Plot-NPC**-Item. Dieses kannst du z. B. im [CaseOpening](../features/das-case-opening.md) gewinnen.

## NPC aufstellen

1. Auf deinem Grundstück an die Stelle gehen, an der der NPC stehen soll.
2. Plot-NPC-Item in die Hand nehmen und Rechtsklick machen.
3. Im Menü „Item einlösen?“ auf „Bestätigen“ klicken.

Der NPC erscheint an deiner Position. Zu Beginn ist er ein Spieler-NPC mit deinem Skin.

{% hint style="warning" %}
Das Item funktioniert nur auf einem Grundstück, das dir gehört. Auf Grundstücken, auf denen du nur Rechte hast, kannst du keinen NPC aufstellen.
{% endhint %}

## NPC bearbeiten

Plot-NPCs kann nur der Besitzer des Grundstücks bearbeiten. Das Menü „PlotNPC bearbeiten“ öffnest du mit **Shift + Rechtsklick** auf den NPC.

Mit `/plotnpc` öffnest du auf deinem Grundstück eine Übersicht aller NPCs, auch auf verbundenen Grundstücken. Mit einem Klick auf einen NPC öffnest du sein Menü.

{% hint style="info" %}
Aus der Übersicht kannst du nur NPCs öffnen, die gerade geladen sind. Ist ein NPC zu weit weg, gehe näher an ihn heran.
{% endhint %}

Im Menü findest du folgende Punkte:

* **Art des NPCs**: Spieler oder ein Tier bzw. Monster
* **NPC-Einstellungen**: Aussehen und Verhalten des NPCs
* **Name des NPCs**: Anzeigename über dem Kopf
* **NPC-Ausrüstung**: Rüstung und Item in der Hand
* **NPC-Funktion**: das Menü, das der NPC beim Anklicken öffnet
* **NPC-Position**: Verschieben und Drehen des NPCs
* **NPC löschen**: entfernt den NPC nach einer Bestätigung endgültig. Das Plot-NPC-Item bekommst du dabei nicht zurück.

{% hint style="info" %}
Nicht jede Einstellung und Funktion ist für jeden Spieler freigeschaltet. Fehlt dir eine Berechtigung, steht das im Menü direkt beim jeweiligen Punkt.
{% endhint %}

### Art des NPCs

Neben dem Spieler-NPC gibt es viele Tiere und Monster als NPC-Art, z. B. Schwein, Creeper, Wolf, Pferd, Dorfbewohner oder Eisengolem. In der Auswahl siehst du nur die Arten, die du bereits freigeschaltet hast.

Weitere Arten schaltest du mit Freischalt-Items frei. Besondere Arten wie Enderdrache, Wither, Skelettpferd oder Ältester Wächter gibt es als **Plot-NPC-Skin**-Item im CaseOpening. Du löst das Item mit einem Rechtsklick ein und bestätigst im Menü „Item einlösen?“.

{% hint style="success" %}
Eine freigeschaltete Art gilt dauerhaft für dich und steht dir bei allen deinen Plot-NPCs zur Verfügung.
{% endhint %}

### NPC-Einstellungen

Welche Einstellungen es gibt, hängt von der Art des NPCs ab:

* **Spieler-NPC:** Skin und Schleichen. Für den Skin schreibst du nach dem Klick den Namen eines Spielers in den Chat.
* **Alle NPCs:** „Spieler ansehen“ (der NPC dreht sich zu Spielern in der Nähe) und ob der Name über dem Kopf angezeigt wird.
* **Arten mit Baby-Form:** Baby-Modus.
* **Weitere Arten:** z. B. Farbe beim Schaf, Größe bei Schleim und Magmaschleim, Sitzen bei Wolf und Ozelot oder Farbe und Typ beim Pferd. Den Charged-Modus beim Creeper schaltest du mit dem Item **Plot-NPC-Option (Charged Creeper)** frei.

### Name des NPCs

Nach dem Klick auf „Name des NPCs“ schreibst du den neuen Namen in den Chat. Der Name darf höchstens **15 Zeichen** lang sein. Farbcodes mit `&` sind möglich und zählen nicht mit.

### NPC-Ausrüstung

Hier gibst du dem NPC Helm, Brustplatte, Hose, Schuhe und ein Item für die Hand. Klicke dazu ein Item in deinem Inventar an. Rüstungsteile landen automatisch im passenden Slot, alle anderen Items in der Hand.

Das Item bleibt dabei in deinem Inventar. Mit einem Klick auf einen belegten Slot entfernst du das Item wieder vom NPC.

### NPC-Funktion

Die Funktion bestimmt, welches Menü sich öffnet, wenn jemand den NPC mit Rechtsklick anklickt.

| Funktion | Das öffnet der NPC |
| --- | --- |
| GS-Bewertungen | die Top-Listen der bestbewerteten Grundstücke |
| Orb-Händler | den Orb-Händler aus dem [Orb-System](../features/das-orb-system.md) |
| Orb-Verkäufer | den Orb-Verkäufer |
| Orb-Statistik | die Orb-Statistik |
| Adventure | die Aufgaben des [Adventurers](../features/das-adventurer-system.md) |
| Händler | das Menü eines Händlers, z. B. des [Admin-Shops](../features/das-adventurer-system.md#der-admin-shop). In der Auswahl steht jeder Händler mit seinem eigenen Namen. |
| Plot Marketplace | die [Immobilienbörse](../features/die-immobilienborse.md) |
| Auktionshaus | das [Auktionshaus](../features/das-auktionshaus.md) |
| Lotterie | die [Lotterie](../features/zufallsbasierte-mechaniken.md#lotterie) |
| Angebotszug | den [Angebotszug](../features/das-case-opening.md#angebotszug) |
| Rand-Schmied | den [Rand-Schmied](grundstuecke-veraendern.md#rand-schmied), mit dem du dir einen eigenen Rand erstellst |

Wählst du eine Funktion mit Shift-Klick, übernimmt der NPC zusätzlich den passenden Standard-Skin und Namen, sofern es einen gibt.

Einige Funktionen wie Adventure, Admin-Shop, Immobilienbörse und Angebotszug schaltest du mit eigenen Freischalt-Items aus dem CaseOpening frei.

{% hint style="warning" %}
Die Funktion kannst du nur **einmal** festlegen. Überlege dir vorher gut, welche Aufgabe dein NPC übernehmen soll.
{% endhint %}

### NPC-Position

Im Menü „NPC-Position“ verschiebst und drehst du den NPC:

* **Pfeile für X, Y und Z:** Ein Klick verschiebt den NPC um **1 Block**, ein Shift-Klick um **0,1 Block**.
* **Nach links oder rechts drehen:** Ein Klick dreht den NPC um **90 Grad**, ein Shift-Klick nur ein kleines Stück.
* **Nach oben oder unten sehen:** ändert die Blickhöhe des NPCs.
* **Zu Spieler bewegen:** setzt den NPC an deine aktuelle Position und übernimmt deine Blickrichtung.

Mit dem **Positions-Stick** bewegst du den NPC direkt in der Welt. Du erhältst ihn in diesem Menü über den Stock „NPC-Position bearbeiten“. Mit Shift + Rechtsklick wählst du den Modus, mit einem Rechtsklick wendest du ihn an.

{% hint style="warning" %}
Du kannst einen NPC nur innerhalb deines Grundstücks verschieben. Positionen außerhalb werden nicht übernommen.
{% endhint %}

## Zugriff auf den NPC

Ohne weitere Einstellung können nur du und Spieler mit [Rechten auf deinem Grundstück](grundstucksrechte-vergeben.md) die Funktion deines NPCs nutzen. Vertraute können das immer, Helfer nur, solange du online bist.

Sollen alle Besucher deinen NPC benutzen können, setzt du die [Flag](../befehlsuebersicht/grundstuecks-befehle/grundstuecks-flags.md) **npc-interact**: `/p flag set npc-interact true`
