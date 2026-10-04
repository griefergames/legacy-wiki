---
description: Befehle für abschließbare Truhen (/chest)
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

# Abschließbare Truhen

Mit diesen Befehlen kannst du die Einstellungen für die [Abschließbaren Truhen](../../features/abschliessbare-truhen.md) verwalten. Schau dafür die abschließbare Truhe auf deinem Grundstück an, bevor du den Befehl eingibst.

| Befehl | Kurzerklärung |
| --- | --- |
| `/chest` | Zeige eine Übersicht aller Befehle an. |
| `/chest trust <Spielername>` | Gib die Truhe für den Spieler frei. |
| `/chest add <Spielername>` | Gib die Truhe für den Spieler frei, solange der Grundstücksbesitzer anwesend ist. |
| <p><code>/chest trust &lt;Spielername> &lt;Zeit m/h/d></code><br>Bsp.: <code>/chest trust AbgegrieftHD 10h</code></p> | Gib die Truhe für eine bestimmte Zeit frei. (Zeit kann frei gewählt werden). |
| <p><code>/chest add &lt;Spielername> &lt;Zeit m/h/d></code><br>Bsp.: <code>/chest add AbgegrieftHD 2d</code></p> | Gib die Truhe eingeschränkt für eine bestimmte Zeit frei. (Zeit kann frei gewählt werden). |
| `/chest remove <Spielername>` | Entziehe dem Spieler den Zugriff auf die Truhe. |
| `/chest remove *` | Entziehe allen Spielern den Zugriff. Danach hast nur noch du Zugriff auf die Truhe. |
| `/chest notification` | Erhalte eine Chatbenachrichtigung beim Öffnen der Truhe (funktioniert nur auf dem jeweiligen Citybuild-Server). |
| `/chest info` | Zeige eine Übersicht der aktuellen Zugriffsrechte an. |
