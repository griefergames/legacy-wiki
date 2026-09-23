---
description: Kartenbauen einfach gemacht
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
  actions:
    visible: true
---

# Vom Bild zur Karte

Moin zusammen, dieses Tutorial befasst mich dem Kartenbau auf der 1.8\
\
Kartenbau besteht grob aus 3 Schritten: 1. Bildauswahl und Erstellung. 2. Umwandeln in entsprechende Vorlagen. 3. Das Ingame-Bauen

### **1. Die Bildauswahl:**

Ohne Bild keine Karte, das ist klar. Aber nach welchen Kriterien wird ein Bild ausgewählt? Dabei gelten 2 grundsätzliche Beschränkungen: Pixelgröße und Farbtiefe.\
\
Eine Karte ist 128x128 Pixel groß. Ein mega-detailreiches Bild werde ich nie fein genug auf einer Karte auflösen können, damit es gut aussieht. Da kann man entgegen wirken, in dem man das Motiv über mehrere Karten baut. Je größer später die Karte, desto mehr Details lassen sich abbilden und desto feiner und klarer werden die Linien.<br>

Wir haben je nach verwendetem Aufwand 16 (Regelfall), 34 oder 102 Farben zur Verfügung. Stark unterschiedliche Farben lassen sich auf Karten wesentlich besser darstellen als Farbverläufe. Hat dein ausgesuchtes Bild zb einen Farbverlauf von Orange zu Gelb? Dann rechne schon mal damit, dass das auf der Karte nicht gut umgesetzt werden kann. Auch hier gibt es Wege das zu kaschieren, das erfordert aber viel Übung und Zeit. Deswegen ist es wichtig, seinen Blick schon bei der Bildauswahl dafür zu schärfen.

Manchmal musst du auch eigene Bilder erstellen, gerade Logos oder Schriftzüge. Hier kannst du schon drauf achten, dass die Schrift nicht zu verschnörkelt wird (Details) oder klare Farben und Abgrenzungen verwendet werden (weiße Schrift mit hellhellgrauem Schatten auf hellgrauem Hintergrund wird man ingame nicht lesen können).

### **2. Umwandeln in Schematic:**

In 1. haben wir unser Bild gefunden. Jetzt muss es Ingame verfügbar werden.\
\
Von vielen wird zuerst Spritecraft gefunden - Ein einfaches PixelArtProgramm, das nicht zur Kartenerstellung geeignet ist (FreakyFreeke hat dazu ein guten Text geschrieben, das spar ich mir hier)

<details>

<summary>Wie man Karten wirklich baut - kein Spritecraft! (by FreyakyFreeke)</summary>

Moin&#x20;

Ich habe mich dazu entschieden dieses Tutorial zu machen, weil es meines Wissens nach, kein Tutorial auf GG gibt, welches das Kartenbauen richtig erklärt.

Erstmal zu Spritecraft und warum es nicht geeignet ist für Kartenbauen. Spritecraft ist ein Pixelart Programm und keins für Maparts! Wo ist der Unterschied? Ein Pixelart Programm liefert euch ein Ergebnis nach der Blockoberfläche. Das geht in vielen Fällen auch gut, aber eben nicht in allen. Es kann passieren, dass euch zwei Blöcke als verschiedene Abstufungen einer Farbe angezeigt werden, obwohl es auf der Karte selbst ein und dieselbe ist. Oder Diorit wird als ein graues weiß verwendet, obwohl es eig ein gelbes weiß und kaum vom normalen weiß zu unterscheiden ist. Und dann gibt es da noch die Blöcke, die eigene Kartenfarben sind, die Spritecraft euch aber nie liefern wird, weil sei transparent sind und damit für Pixelart ungeeignet, wie Spinnenweben, Wasser oder Eis.

Nun zu den Mapart Programmen. Sie gehen nur danach, welche Farbe der Block am Ende auf der Karte liefert. Dies ermöglicht es euch auch schemtaics für 3D-Karten zu bekommen, die jedoch wesentlich komplexer im Aufbau sind. Ein bisschen mehr Erklärung wie die Programme arbeiten und wie Minecraft Karten funtkionieren findet ihr hier:

[https://minecraft.gamepedia.com/Map\_item\_format](https://minecraft.gamepedia.com/Map_item_format)

Ich persönlich nutze für den Kartenbau den ersten Eintrag bei Google für Mc Maparts: MapartCraft.

#### Wie MapartCraft funktioniert

Links könnt ihr dort die Blöcke auswählen, die ihr für die jeweilige Farbe verwenden wollt. Bitte bedenkt hierbei, dass GG auf der 1.8 läuft und alles ab dem gebrannten Ton euch nichts bringt. Da gebrannter Ton in der 1.8 dieselbe Farbe wie Wolle hat.

Rechts könnt ihr euer Bild einfügen und ein paar weitere Einstellungen vornehmen, die ich euch einmal der Reihe nach vorstellen möchte.

Mode: Hier könnt ihr eine map.dat Datei bekommen, die ihr in eine Singleplayer Welt oder auf euren eigenen Server einfügen könnt. Oder ihr entscheidet euch für die NBT Datei, die könnt ihr mit Schematica in der 1.12 öffnen, jedoch nicht in der 1.8.

MapSize: Eigentlich selbsterklärend, hier stellt ihr die Größe eurer Karte ein

Grid: Gitternetz anzeigen

Staircasing: Hier stellt ihr ein ob ihr eure Karte 2D oder 3D bauen wollt.

Bettercolor: Liefert euch ein anderes Farbenbild. Testet einfach aus, ob es bei eurem Bild besser oder schlechter aussieht.

Dithering: Hier stellt ihr ein wie die Karte umgewandelt werden soll, probiert euch da einfach mal alles aus.

Add Blocks under: Wie viele Hilfsblöcke wollt ihr setzten

Block to add: Welchen Block wollt ihr als Hilfsblock setzten

ImagePreProcessing: Weiterer Einstellungskram, wie Helligkeit oder Kontrast

Wenn ihr nicht eine große Datei wollt könnt ihr auch den Button unter dem Download anklicken, dann kriegt ihr für jede Karte eine einzelne Schematic.

So viel zu dem Programm. Es sei jedoch dazu gesagt das, auch wenn Maparts besser funktionieren, man nicht umhin kommt seine Karte noch zu bearbeiten. Angefangen damit, dass ihr euer Bild richtig skaliert, damit es nicht verzerrt wird und die Details nicht verloren gehen, bis dahin, dass ihr nochmal hingeht und die Details nachbessert.

Da das hier aber den Rahmen sprengen würde, erkläre ich euch nur noch kurz an einem Beispiel, wie man richtig skaliert, da ich das schon häufiger gefragt wurde.

#### Skalieren

Das Bild ist 728x1122 hat also ein Seitverhältnis von 728:1122= 1,54. Ich wähle eine Kartengröße mit einem ähnlichen Seitenverhältnis wie z.b. 2x3 mit 1,5, 3x5 mit 1,67 oder 4x6 mit 1,5. Wir nehmen hier mal 3x5. Nun entscheiden wir uns wo wir am Rand vom Bild noch ein bisschen was wegschneiden wollen (tipp: ihr könnt natürlich auch ein bisschen was hinzufügen). Wir entscheiden uns für den rechten Rand. Also Teilen wir die Höhe durch die Anzahl der Karten und multiplizieren mit der Anzahl der Karten, der Breite: 1122/5=224,4 (wir wollen keine angebrochenen Pixel also rechnen wir mit 224 weiter) 22&#x34;_&#x33;=672. Ich wähle also einen Ausschnitt der Karte, der 22&#x34;_&#x35;X224x3 also 672x1120 groß ist. (Noch ein Tip wenn ihr richtig skaliert habt, zeigt euch MapartCraft die Zahl unter dem Bild nichtmehr rot an.)

#### Wie man Karten verbessert - Ein kleiner Einblick

Vorweg ich versuche Karten immer möglichst ohne Dithering zu bauen, kann also auch nur dafür Tipps geben. Ihr werdet so jedoch keine Karten mit krassen Lichteffekten hinkriegen, meisten nicht mal wenn ihr 3D baut, dafür ist die Farbpalette in MC einfach zu klein. Ich kann auch leider nicht allzu sehr ins Detail gehen. Es ist einfach sehr viel Erfahrung und ausprobieren. Aber ich kann euch ein paar Tipps geben was man alles ausprobieren kann und wie man meiner Meinung nach am besten pixelt.

Farben sind in Minecraft ein riesen Problem ihr habt insgesamt 35 Kartenfarben. Davon sind 9 Schwarz-Weiß Töne, aber es gibt zB nur ein Orange. Das bedeutet für uns als Kartenbauer, dass es immer leichter ist in schwarz-weiß zu bauen. Ein weiteres großes Problem gerade, wenn man ohne Dithering baut sind Hautfarben, weil es einfach keine gibt. Die kommen leider erst mit der 1.12 ins Spiel. Ihr müsst verstehen, wo die Grenzen eurer Farbmöglichkeiten liegen, um gute Karten bauen zu können.

Aber nun zurück zum Anfang. Mein erster Tipp ist, nehmt ein Bild mit guter Auflösung. Selbst wenn ihr nur eine 1er Karte baut, kann das Bild gerne 500x500 Pixel sein. Mapartcraft wird euch dann viel bessere Ergebnisse liefern.

Spielt ein bisschen mit den Einstellungen, bringt Bettercolor mehr oder sieht es schlechter aus? Ihr könnt auch beim Dithering Bayer oder Ordered benutzen um nachhinein die Pixel mehr verbinden. Meistens ist dort die Farbgebung schöner. Ihr könnt auch noch mit den Blöcken herumexperimentieren, die das Programm verwenden darf. Wenn ihr zb eine rote Fläche habt, die aber rosa übersetzt wird, könnt ihr rosa als Farbe einfach rausnehmen. Oder wenn Sprenkel einer Farbe im Bild sind, die nicht reinpassen, könnt ihr diese ebenfalls einfach entfernen.

Ich empfehle es nicht Helligkeit oder Kontrast auf der Website zu benutzen, nehmt dafür lieber ein externes Fotoprogramm und spielt auch hier ein bisschen mit den Einstellungen und lasst die Bilder dann als Karten übersetzten, um zu gucken, was für euch das beste Ergebnis ist.

Nun zum bearbeiten selbst. Wenn ihr rechtsklick auf die Vorschau macht, könnt ihr diese abspeichern und mit anderen Programmen nachbearbeiten. Ich benutze hierfür Gimp, da es mehr Möglichkeiten hat, empfehle Einsteigern aber vll erstmal Paint. Wichtig ist, dass ihr, wenn ihr das Bild öffnet um es zu bearbeiten, dabei nur die Farben benutzt, die auf dem Bild sind, oder die Ihr in der Farbpalette findet. (Ich lade sie euch unten nochmal hoch). Den Vorteil den ich am Bearbeiten mit einem Programm sehe, ist ihr seht sofort euer Ergebnis im Gesamtbild. Wenn mal etwas nicht so klappt, wie ihr es wollt, empfehle ich immer nochmal einen Blick ins Original, zu werfen um zu gucken, wie es da umgesetzt wurde. Hier jetzt ins Detail zu gehen was man genau macht findet ich schwierig, weil es sehr vom Bild abhängt. Ich würde zb Farbgebung korrigieren, teile vom Bild die unscharf geworden sind per Hand nach pixeln (je nach Bild muss man aufpassen, dass es nicht zu gemalt aussieht) oder etwas komplett Eigenes daraus kreieren. Der Vorteil ist, ihr macht es nicht in MC selber und könnt so mit wenigen Klicks viel ausprobieren oder es auch ganz schnell wieder rückgängig machen. Speichert euch aber vll ein paar Zwischenstände, falls ihr doch mal was versaut.

Mein letzter Tipp fang mit etwas Leichtem an. Nehmt ein Bild bei dem ihr nur Kleinigkeiten korrigieren müsst oder das sehr einfach in Form und Farbe ist wie zb ein Pokemon. Wachst lieber langsamer als am Ende überfordert zu sein und wenn ihr ein Bild mal nicht mehr sehen könnt macht eine Pause. Fragt vll auch Freunde, wenn ihr euch nicht sicher seid, was besser aussieht. Und auch wenn ihr, nun da ihr ein Programm für Maparts benutzt, genau wisst wie eure Karte später aussieht, schaut sie euch, wenn sie aufgebaut ist trotzdem noch einmal im Detail an um Baufehler oder Pixelfehler die ihr vorher übersehen habt zu vermeiden.

</details>

Das Programm - oder viel mehr die Webseite - die alle mir bekannten Kartenbauer nutzen ist [https://rebane2001.com/mapartcraft/de](https://rebane2001.com/mapartcraft/de)\
Hier könnt ihr euer Bild einfach reinladen, diverse Einstellungen verändern und bekommt das Vorschaubild direkt gerendert. Hier passiert auch die eigentliche Kunst des Kartenbaus. Es kommt vor, dass ich tagelang an einer Grafik sitze bis ich zufrieden bin. Manchmal ist es nötig, das eigentliche Bild noch ein wenig zu "frisieren", wenn das eine oder andere Detail nicht ganz so passt, wie man es gerne hätte.

<details>

<summary>Mapart-Einstellungen</summary>

Format: Schematic (NBT)

Version: 1.12.2

Maße: a x b --> darfst du frei wählen, a ist dabei die Breite, b die Höhe

Zuschneiden: Center (in der Regel passt das, wenn du nur einen Bildausschnitt haben willst kannst du hier auf Manuell gehen und reinzoomen)

Grid: off

Staircasing: Off (On ist auch möglich, dann wirds aber ne aufwändige 3D-Karte)

Platziere Blöcke unter: Off (Wird nur bei 3D-Karten benötigt)

Platzierter Block: Cobblestone (Bezieht sich auf das platziere Blöcke unter)

Verbesserte Farben: On (Je nach Karte kannst du das auch ausschalten

Dithering: das Farb-berechnungs-Verhalten. Hier kannst du dich austoben

Image preprocessing: Hier kannst du Helligkeit, Sättigung und Kontrast der gesamten Grafik anpassen. Hintergrundverwendung ist eine reine 3D-

Einstellung und hat im 2D-Bereich nichts verloren.

</details>

<details>

<summary>Farben/Materialien</summary>

Alle Materialien, laut /p h color, cb3

* Obsidian, Kohleblock, schwarzes Glas, schwarze Keramik, schwarze Wolle
* graue Keramik, graues Glas, graue Wolle
* Stein, alle Erze, gemeißelter Steinziegel, Steinziegel, bemooster Stein, Akazie liegend, ec, Kolben, Werfer, Spender, Trichter, Kies, Andesit (+poliert), Bruchstein
* Clay
* Schwarzeiche liegend + Bretter, Fichte liegend, Seelensand, braunes Glas, braune Keramik, braune Wolle
* Fichte stehend + Bretter, Trope liegend, Eiche liegend, Podsol
* Trope stehend + Bretter, Plattenspieler, Granit (+ poliert), Erde, grobe Erde, brauner Pilzblock
* Eiche stehend + Bretter, Werkbank, Truhe, Bücherregal
* Akazienlaub, Birkenlaub, Fichtennadeln, Eichenlaub, Schwarzeichenlaub, Tropenlaub
* Smaragdblock
* grünes Glas, grüne Wolle, grüne Keramik
* Melonenblock, hellgrünes Glas, hellgrüne Wolle, hellgrüne Keramik
* Grasblock, Schleimblock
* Prismarin, türkise Wolle, türkises Glas, türkise Keramik
* Prismaziegel, Diablock, Beacon, dunkler Prismarin
* blaue Wolle, blaue Keramik, blaues Glas
* Lapisblock
* hellblaue Wolle, hellblaue Keramik, hellblaues Glas
* Packeis, Eis
* Myzel, violettes Glas, violette Keramik, violette Wolle
* magenta Wolle, magenta Keramik, magenta Glas
* rosa Glas, rosa Wolle, rosa Keramik
* Netherziegelstein, Quarzerz, Netherrack
* Redstoneblock, Lava
* Zaubertisch, roter Pilzblock, Ziegelstein, rote Wolle, rote Keramik, rotes Glas
* Akazie stehend + Bretter, Kürbis, roter Sand, oranges Glas, orange Wolle, orange Keramik
* nasser Schwamm, trockener Schwamm, Heuballen, gelbes Glas, gelbe Wolle, gelbe Keramik
* Goldblock
* Sandstein, gemeißelter Sandstein, glatter Sandstein, Birke stehend + Bretter, Glowstone
* hellgraue Keramik, hellgraues Glas, hellgraue Wolle
* Eisenblock, Braustand
* Spinnweben, Bett
* Schneeblock, weiße Wolle, weiße Keramik, weißes Glas
* Seelaterne, gemeißelter Quarz, Quarzblock, Quarzsäule, Birke liegend

Alle hier gelisteten Materialien lassen sich 1:1 gegeneinander austauschen.

Wenn du mit den 16 Wollefarben baust ist es sinnvoll, die vollen Blöcke in der Auswahl durch Teppiche zu ersetzen. Das spart später Arbeit.

</details>

Wenn du mit der Vorschau deiner Karte in Mapart soweit zufrieden bist, hast du 2 Möglichkeiten:

Über die Schaltfläche "Download" lädst du die komplette Schematic an einem Stück herunter (nur ratsam bei kleinen 1er-Karten)

Über die Schaltfläche "Download als 1x1-Teile" bekommst du die Kartenteile automatisch in Kartenplot-gerechte Schematicen aufgeteilt.

Je nach dem, welche Variante du wählst ist es nötig, die nun heruntergeladenen Dateien zu entpacken und vom .MAP in das .SCHEMATIC-Format zu konvertieren. Dazu hat Gleichstand schon ein Tutorial geschrieben, das spar ich mir an der Stelle:

<details>

<summary>Schematics einfach im Browser bearbeiten - Cubical.xyz (by Gleichstand)</summary>

Hey liebe Community,

vorerst checken wir folgende Dinge:

**Was ist Cubical.xyz?**

Es ist eine im Webbrowser aufrufbare Webseite, bei der man eine Schmeatic-Datei einfügen und bearbeiten kann. So kann man beispielsweise Blöcke oder ganzes Terrain umändern. Man spart sich somit eine menge Zeit.

**Was wird erklärt?**

Ich erkläre euch hier, wie die einzelnen Befehle der Webseite funktionieren.

Da die allgemeine Hilfe der Webseite nur auf Englisch existiert, ist es hier auf deutsch erklärt.

Das Ganze funktioniert so ähnlich wie WorldEdit.

**Link:** [https://cubical.xyz/](https://cubical.xyz/)

Hier unten sind alle Befehle, somit Nutzungen der Webseite erklärt.

#### Schematic hochladen und herunterladen

Wenn die Webseite geöffnet ist, klickt man oben links auf ''Datei'' und wählt mit ''Datei öffnen'' die jeweilige Schematic-Datei aus. Ist das Ganze geöffnet, kann man diese nun bearbeiten.

Um sie nach Bearbeitung zu speichern, wieder oben links auf ''Datei'' klicken und auf ''Exportdatei'' , dann auf ''Schematische Datei'' klicken. Es wird dann automatisch eine Schematic-Datei gedownloadet. Diese ist im Ordner ''Downloads'' zu finden.

#### Allgemeine Hinweise

| Sie können mit der Maus auf fast allen Zahleneingabefeldern scrollen, um die angegebenen Werte zu erhöhen oder zu verringern.                                                                             |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Fenster rasten ein, wenn sie in der Nähe des Randes eines anderen Fensters oder Bedienfelds verschoben oder in der Größe geändert werden. Dies kann durch Halten der Alt-Taste deaktiviert werden.        |
| Windows kann durch Doppelklicken auf die obere Titelleiste minimiert werden.                                                                                                                              |
| Die Hauptfensteransicht kann durch Doppelklicken auf die obere Symbolleiste umgeschaltet und maximiert werden                                                                                             |
| Sie können das Blockauswahlfenster auf drei Arten öffnen, indem Sie die Taste 'b' drücken, auf die Aktionsleiste doppelklicken oder auf eine Materialeingabe in einem beliebigen Werkzeugfenster klicken. |
| Blöcke und Werkzeuge können um die Aktionsleiste an bestimmte Positionen gezogen oder in den Hauptansichtsbereich gelegt werden, um sie vollständig zu entfernen.                                         |
| Durch Klicken auf den Dateinamen unten links in der Statusleiste können Sie die aktuell geöffnete Datei umbenennen oder ihre Größe ändern.                                                                |

#### Auswahlwerkzeuge

<table data-header-hidden><thead><tr><th width="212"></th><th></th></tr></thead><tbody><tr><td>Auswahlwerkzeuge</td><td>Mit den Auswahlwerkzeugen können Sie einen bestimmten Quaderbereich ändern, erstellen oder bearbeiten. Sobald ein Auswahlwerkzeug aktiv ist, kann der Benutzer mit der linken Maustaste die Eckenpositionen des gewünschten Bereichs umschalten. Nach der Auswahl können Sie das Tool über den aktuellen Bereich ausführen, indem Sie auf die Schaltfläche "Ausführen" klicken.</td></tr><tr><td>Benutzerdefinierte Filter</td><td>Mit dem benutzerdefinierten Filter können Sie wie mit den benutzerdefinierten Pinsel- und Generatorwerkzeugen Ihre eigene benutzerdefinierte Skriptlogik angeben, um zu steuern, wie und was der Filter tut. Sie können den kleinen Textbereich für das Skript verwenden oder das Kontrollkästchen verwenden, um das benutzerdefinierte Skriptfenster zu aktivieren und zu öffnen, in dem benutzerdefinierte Skripte und ein viel größerer Bearbeitungsbereich gespeichert werden können.</td></tr><tr><td>Auswahl kopieren</td><td>Mit dem Auswahlwerkzeug können Sie den aktuell ausgewählten Bereich in die Zwischenablage kopieren, um ihn mit dem Pinselwerkzeug zum Einfügen zu verwenden.</td></tr><tr><td>Auswahl füllen</td><td>Das Füllwerkzeug macht genau das, was der Name schon sagt, und füllt den Auswahlbereich. Die einzige Eingabe außer dem Auswahlfeld ist der Block, der für die Füllung verwendet werden soll.</td></tr></tbody></table>

#### Brush Werkzeuge

<table data-header-hidden><thead><tr><th width="179"></th><th></th></tr></thead><tbody><tr><td>Brush Werkzeuge</td><td>Um sie zu verwenden, müssen Sie ein Pinselwerkzeug im Menü auswählen, dann die gewünschten Parameter einstellen und dann auf das Werkzeugsymbol doppelklicken oder es in die Aktionsleiste ziehen, wo es für Links- und Rechtsklick-Interaktionen innerhalb des Menüs verwendet werden kann Welt.</td></tr><tr><td>Block Brush</td><td>Das Blockbürstenwerkzeug ist das Standardwerkzeug, das beim Platzieren eines einzelnen Blocks verwendet wird. Es wird automatisch ausgewählt, wenn ein beliebiger Block in der Aktionsleiste verwendet wird, und verfügt nur über eine einzelne Blockmaterialeingabe.</td></tr><tr><td>Bump Brush</td><td>Der Bump-Pinsel ist ein Bearbeitungswerkzeug, das die Oberfläche des angeklickten Objekts verformt. Er wird normalerweise bei Terraforming-Operationen verwendet. Eine Gesamtgröße und Festigkeit steuert, wie groß eine Fläche ist und wie viel Verformung auftritt. Positive Werte erhöhen die Oberfläche, während negative Werte abnehmen.</td></tr><tr><td>Custom Brush</td><td>Mit dem benutzerdefinierten Pinselwerkzeug können Sie Ihre eigene Steuerlogik festlegen, wenn der Pinsel verwendet wird. Wie die anderen Generator-Tools verfügt es über einen grundlegenden Skriptbereich sowie ein detaillierteres Skriptbearbeitungsfenster, das mit dem Kontrollkästchen umgeschaltet werden kann.</td></tr><tr><td>Erode Brush</td><td>Das Erodierbürstenwerkzeug ist ein Bearbeitungsverformungswerkzeug, das normalerweise zum Bereinigen oder Glätten von Geländebearbeitungsvorgängen verwendet wird, die von anderen Werkzeugen übrig geblieben sind. Sie können den zu glättenden Bereich zusammen mit der Anzahl der offenen Flächen steuern, die zum Löschen eines bestimmten Blocks erforderlich sind.</td></tr><tr><td>Fill Brush</td><td>Das Füllbürstenwerkzeug funktioniert wie das Erodieren bis, jedoch in entgegengesetzter Weise. Es werden Lücken zwischen Blöcken platziert oder gefüllt und Kanten vergrößert. Die Größe und Anzahl der zum Ausfüllen erforderlichen Flächen kann eingestellt werden, um eine größere Vielfalt an Festigkeiten und Oberflächen zu ermöglichen.</td></tr><tr><td>Overlay Brush</td><td>Das Überlagerungspinsel-Werkzeug ist ein weiteres Werkzeug, das hauptsächlich bei der Geländebearbeitung verwendet wird. Sie können mehrere Ebenen von Blöcken angeben und festlegen, die den angeklickten Bereich überlagern oder ersetzen. Es können bis zu drei verschiedene Schichtmaterialien und Schichttiefen spezifiziert werden, zusammen mit der Möglichkeit, die Änderungen nur auf natürliche Blöcke zu beschränken.</td></tr><tr><td>Sphere Brush</td><td>Das Kugelpinselwerkzeug ist ein einfaches Füllwerkzeug, mit dem der Benutzer eine Kugel des ausgewählten Blocks an der angeklickten Stelle platzieren kann. Sie können den Luftblock verwenden, um auf die gleiche Weise zu löschen.</td></tr><tr><td>Tree Brush</td><td>Der Baumpinsel ist ein Werkzeug, mit dem Sie mehrere verschiedene Baumarten platzieren können, wo immer Sie klicken. Verschiedene Einstellungen ermöglichen das Ändern des Blatt- und Holzmaterials zusammen mit der Baumart und der Gesamtgröße. Den meisten Bäumen werden zufällige Variationen hinzugefügt, um die Anzahl der produzierten Duplikate zu verringern.</td></tr><tr><td>Paste Brush</td><td>Mit dem Einfügepinsel können Sie Formen platzieren, die in die Zwischenablage kopiert wurden.</td></tr><tr><td>Grass Brush</td><td>Die Grasbürste erzeugt eine Überlagerung von natürlichen Laubblöcken über dem aktuellen Gelände. Mit dem Dichte-Parameter können Sie die Gesamtdichte der zu platzierenden Gras- und Blumenblöcke angeben.</td></tr><tr><td>Vine Brush</td><td>Die Weinbürste ist ein spezielles Werkzeug, mit dem der Benutzer Weinreben auf einfach zu verwendende Weise platzieren kann. Sie können die Dichte der Rebplatzierung, einen alternativen zu verwendenden Rebblock oder festlegen, ob Reben an einer Seitenwand oder nur an Kanten platziert werden sollen, dh keine Blöcke unter der Wand.</td></tr><tr><td>Flood Brush</td><td>Das Flutbürstenwerkzeug ist sehr nützlich, wenn Sie Bereiche desselben Blocktyps ersetzen. Der Größenparameter steuert die maximale Entfernung, über die sich die Flut ausbreiten kann, während der Lückenparameter steuert, wie nahe die Blöcke desselben Typs sein müssen, um die Flut fortzusetzen. Die Flut beginnt mit dem ersten angeklickten Block und wird sich weiter ausbreiten und die Blöcke ersetzen, bis sie ein Limit erreicht.</td></tr></tbody></table>

#### Generator Tools

| Generator Tools   | Der Hauptunterschied zwischen den Generatorwerkzeugen und den anderen besteht darin, dass das Generatorwerkzeug beim Ausführen immer eine neue Datei erstellt. Einige Werkzeuge haben eine Größeneinstellung, während andere basierend auf anderen Parametern des Werkzeugs festgelegt werden.                                                                                                                                                                                                                                                                                                                                                                                                                    |
| ----------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 3D Text Generator | <p>Parameterdefinitionen<br>[Text Depth] Texttiefe Die Anzahl der Blöcke, die die 3D-Texttiefe betragen soll.<br>[Edge Inset] Die Anzahl der Blöcke, in die die Kante eingerückt werden soll.<br>[Font Size] Die Größe der Schriftart, die bei der Texterstellung verwendet werden soll.<br>[Font] Die Art der Schriftart, die für die Texterstellung verwendet werden soll.<br>[Main Block] Die Art des Blocks, den der Hauptteil des Textes haben sollte.<br>[Outline Block] Die Art des Blocks, den der Gliederungsteil des Textes haben sollte.</p>                                                                                                                                                           |
| Custom Generator  | <p><br>Mit dem benutzerdefinierten Generator können Sie Ihre eigene benutzerdefinierte Skriptlogik angeben, um zu steuern, wie und was der Generator erstellt. Sie können die Höhe, Breite und Länge des Bereichs angeben, der beim Ausführen generiert werden soll.<br>Sie können den kleinen Textbereich für das Skript verwenden oder das Kontrollkästchen verwenden, um das benutzerdefinierte Skriptfenster zu aktivieren und zu öffnen, in dem benutzerdefinierte Skripte und ein viel größerer Bearbeitungsbereich gespeichert werden können.</p>                                                                                                                                                          |
| Terrain Generator | <p>Parameterdefinitionen<br>[Width] Die Anzahl der Blöcke, die im Genbereich breit sein sollten.<br>[Height] Die maximale Anzahl von Blöcken, die der Genbereich betragen sollte, sollte sein.<br>[Depth] Die Anzahl der Blöcke, die tief im Genbereich liegen, sollte sein.<br>[Octaves] Diese Zahl definiert die Intensität oder Detailstärke des Rauschens (niedriger = weniger Intensität; höher = mehr Intensität)<br>[Falloff] Hiermit wird gesteuert, wie schnell sich die Höhe des Geländes ändern kann. (niedriger = glatter; höher = gezackter)<br>[Cycles] Dies steuert die Gesamtgröße oder Anzahl der Zyklen. (niedriger = detaillierter oder hügelig; höher = weniger detailliert oder glatter)</p> |



Ich hoffe, dass ich weiterhelfen konnte.

Grüße,

Gleichstand

</details>

Anschließend die Schematic-Dateien noch in den entsprechenden Schematics-Ordner verschieben und du kannst theoretisch ingame loslegen.

### **3. Karte Ingame bauen**

#### **3.1 Das Kartenplot:**

Zu allererst braucht es ein Kartenplot. Weiter oben wurde ja schon erwähnt, dass eine Karte 128x128 Pixel groß ist, genau so groß muss auch das Plot sein. Das sind auf GG mindestens 4x4 Plots. Die dürfen aber nicht irgendwo sein, sondern müssen im Kartenchunk liegen.

<details>

<summary>Kartenchunk und wie ich ihn finde</summary>

Der Chunk ist die Basis-Speichereinheit von Minecraft und besteht aus 16x16 Blöcken und geht über die ganze Höhe. Eine Karte bildet immer 8x8 Chunks ab (der Einfachheit halber Kartenchunk genannt). Genau wie Chunks selbst, lassen sich die Kartenchunks nicht verschieben.

Um einen Kartenchunk zu finden brauchst du ein paar Blöcke und leere Karten:

1\. Du läufst/fliegst in eine unbebaute Gegend und claimst ein GS. Du kannst den Rand für bessere Erkennbarkeit ändern.

2\. Du ziehst eine Karte von deinem unbebauten GS.

3\. im optimalen Fall sind 16 GS auf der Karte sichtbar und am Rand der Karte keine Straße. Dein GS kannst du am farbigen Rand auf der Karte erkennen. Wenn mehr GS auf der Karte sichtbar sind oder eine Straße am Kartenrand verläuft musst du in dieser Richtung eine Reihe mehr GS claimen und Mergen, so dass nachher keine Straße mehr auf der Karte sichtbar wäre/ist. Mit etwas Vorstellungskraft und Übung reicht eine gezogene Karte um ein Kartenplot zu erstellen, es ist aber auch nicht falsch nach jedem Schritt eine neue Karte zu ziehen und den Fortschritt zu überprüfen.

</details>

Die Chunkgrenzen zeigen dir jetzt an, wo der Kartenchunk endet. Auf der 1.8 sind die etwas schwer zu finden, über f3 und den Debugg-Screen lassen sie sich aber finden. Wenn die Zahl bei Chunk (linke Seite, zweiter Block von oben, dritte Zeile) von 15 auf 0 umschlägt hat man die Grenze gefunden. Einen Block außerhalb der Kartenfläche, so dass es gerade nicht mehr auf der Karte sichtbar ist, platzierst du jetzt eine Reihe Steine oder andere Blöcke, den sogenannten Kartenrand.

<details>

<summary>Drunken1990 hat ein Tutorial mit Video-Erklärung erstellt:</summary>

Hallo liebe Griefergames Community,

Es kamen sehr häufig Fragen, wie man denn ein Kartenplot erstellt. WIe man die position findet und wie man dann richtig merged. Ich habe mal einen Videoguide dazu gemacht. Falls aber noch Fragen offen sind, scheut euch nicht zu fragen. Viel Spaß mit dem Video. Hoffe, ich konnte euch helfen&#x20;

Euer Drunken1990

{% embed url="https://www.youtube.com/watch?v=3WMTxrjMhfg" %}

</details>

Jetzt kannst du deine Schematic laden und mit Bauen anfangen.

Alternativ kannst du auch fertige Kartenplots mieten oder bauen lassen.

#### **3.2 Spülanlage und Automatisches Lager:**

Irgendwann ist die Karte fertig und gezogen - jetzt muss wieder abgebaut werden. Wenn du deine Karte mit Teppichen gebaut hast kannst du sie mit Wasser wegspülen und die Teppiche mit Trichtern unter der Kartenfläche einsammeln und automatisch wegsortieren lassen. Das geht alles über Knopfdruck, spart dir Arbeit und beschleunigt den Kartenbau.

Das Lager sollte im Idealfall 5 DK pro Farbe/Material beinhalten. Damit kann eine volle einfarbige Karte gelegt werden.

Bei den Spülanlagen ist es ratsam, nicht über einen Knopf die komplette Fläche zu spülen, sondern die Fläche zu vierteln. Das hängt mit der maximalen Sichtweite auf GG zusammen und verhindert, dass das Wasser am Sichtweitenende anfängt zu buggen.

***

{% hint style="info" %}
Hast du deine Karte fertig und möchtest sie vor Kopien schützen, kannst du das mit dem Befehl /anticopy erledigen, wenn du die Karte in der Hand hältst. Du kannst diesen Schutz jeder Zeit mit der erneuten Eingabe des Befehls entfernen.
{% endhint %}



<details>

<summary>An diesem Artikel beteiligt</summary>

* [DeGabo](https://profile.griefergames.net/minecraft/d859e005-af4a-40af-bc56-351d36cf4a96)
* [FreakyFreeke](https://profile.griefergames.net/minecraft/02525716-d607-462a-bd86-c2894cb589e4)
* [Gleichstand](https://profile.griefergames.net/minecraft/a3122920-03df-428c-8886-f1e142c1767b)
* [Drunken1990](https://profile.griefergames.net/minecraft/002147e7-a675-4732-afd3-86c6495df6ee)

</details>
