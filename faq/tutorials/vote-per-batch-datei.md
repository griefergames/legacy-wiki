---
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
    visible: false
  tags:
    visible: true
---

# Vote per Batch-Datei

Hey Leute!

Ich vote seit langem per Batchdatei, da es gerade mit mehreren Accounts um einiges einfacher ist. Dazu hab ich folgende Zeilen in meiner Batchfile:

**Code**

{% code lineNumbers="true" expandable="true" %}
```
@Echo off
start https://minecraft-server.eu/vote/index/1A73C/phanTom84_
timeout /t 1
start https://minecraft-server.eu/vote/index/1A73C/miniTom6077
timeout /t 1
start https://minecraft-server.eu/vote/index/1A73C/leo_nie07
stop
```
{% endcode %}

#### Wie könnt ihr so eine Batch erstellen?

Öffnet den ganz normalen Editor von Windows _(Windowstaste + R und dann notepad.exe eingeben)_ und beginnt mit dem Befehl <kbd>@Echo off</kbd>. \
Darunter kommt dann zuerst der Befehl zum ausführen <kbd>start</kbd> und dann der Link zu einer Vote-Seite <kbd>https://minecraft-server.eu/vote/index/1A73C/</kbd> (dieser ist immer gleich) und am Ende des Links fügt ihr euren InGame-Namen hinzu.

#### Mit mehreren Accounts voten

Vorweg: Es können pro IP Adresse nur 3 Votes abgegeben werden!

Um noch weitere Votes (bis zu 3 eben) hinzuzufügen, geht ihr in die nächste Zeile und gebt wie bei mir im Code oben den Befehl <kbd>timeout /t 1</kbd> ein. Dieser bewirkt, dass zwischen dem ersten aufrufen der Vote Seite und dem nächsten 1 Sekunde Pause ist, da ansonsten nur der erste Link richtig funktioniert. Es wird zwar die Seite aufgerufen und der Name eingetragen in das Feld, aber das Voten funktioniert dann nicht. Mithilfe des `timeout`-Befehls umgeht ihr das Problem.

#### Speichern der Batch-Datei

Habt ihr nun alle Links eingefügt, kommt am Ende noch ein <kbd>stop</kbd>, der die Batch wieder beendet und schließt und ihr geht auf _Datei >> Speichern unter_.

Jetzt wählt ihr einen Speicherort aus und einen Namen für die Datei. Wichtig ist nun, dass erstens auch die Dateiendung <kbd>.bat</kbd> im Feld Dateiname hinzugefügt wird UND zweitens, dass der gesamte Name inkl. der Dateiendung unter Apostroph gestellt werden, da ansonsten einfach eine normale Textdatei und keine ausführbare Batch Datei erstellt wird. Als Dateiname sollte es dann zB. so aussehen: <kbd>"minecraft\_links.bat"</kbd>.

#### Was kann ich noch in die Batch-Datei schreiben?

Ihr könnt natürlich nicht nur die Vote-Links hineinschreiben, sondern könnt auch jegliche andere Links schreiben die ihr öffnen wollt. Einfach in je eine Zeile <kbd>start \<URL der Website die geöffnet werden soll></kbd> schreiben und diese wird gleich mit geöffnet.&#x20;

_Der timeout Befehl ist hierbei nicht nötig!_

Ihr könnt natürlich auch noch den Minecraft Launcher oder sonst eine Programm, Bild oder was ihr sonst am PC/Notebook habt starten. Dazu anstelle des Links einfach den Dateipfad und die Datei samt Dateiendung schreiben. Habt ihr den MC Launcher auf dem Standardpfad von Windows, wäre das zB. <kbd>C:\Program Files (x86)\Minecraft Launcher\MinecraftLauncher.exe</kbd>.

Wichtig ist einfach, dass das <kbd>stop</kbd> erst am Ende der gesamten Batchfile kommt.

#### Batch starten

Wenn ihr nun auf die Batch File doppelklickt, öffnet sich der Browser und die eingegebenen Links sowie Programme und Dateien werden geöffnet. Dann müsst ihr nur mehr auf den Vote-Seiten auf den blauen "Vote"-Button drücken und ihr seid fertig.

<details>

<summary>An diesem Artikel beteiligt</summary>

* [phanTom84\_](https://profile.griefergames.net/minecraft/f856eab9-1212-4d79-9558-e3b3f829a4f3)
* [50U7R34P3R](https://profile.griefergames.net/minecraft/8e2ce0be-aa2c-46a7-a2dc-48f948743edf)

</details>
