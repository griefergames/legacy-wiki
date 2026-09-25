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
  actions:
    visible: true
  anchors:
    visible: true
---

# Praktische Chat-Filter für LabyMod

Hey, ich habe hier ein paar praktische Filter für GrieferGames (Version 1.8) erstellt.

Falls du noch nicht weißt, wie du Filter einrichtest, klicke einfach auf deine Version für das passende Tutorial. Wenn du dich bereits auskennst, kannst du diesen Schritt überspringen: [**LabyMod 3**](https://youtu.be/XtLyDoapibA?t=62) | [**LabyMod 4**](https://youtu.be/XtLyDoapibA?t=180)

## Filter einrichten (kurzes Text-Tutorial)

### Bei LabyMod 3

Um einen Filter einzustellen, drücke "T", um den Chat zu öffnen. Klicke dann unten rechts auf "Chat-Filter", um die gewünschten Filter anzupassen.

**Hinweis:** Bei LabyMod 3 musst du möglicherweise den Filter zuerst aktivieren. Drücke "ESC", gehe zu LabyMod, suche nach "Filter" und aktiviere ihn dort.

### Bei LabyMod 4

Öffne den Chat und klicke auf die drei Striche. Wähle dann "Filter-Einstellungen", um die Filter anzupassen.

## Die Filter

Ich habe dir die wichtigsten Filter vorbereitet, die du ganz einfach kopieren und einfügen kannst. Zudem empfehle ich dir, den **Secondary Chat** zu verwenden oder bestimmte Nachrichten auszublenden – bei den einzelnen Filtern habe ich meine Empfehlung (**Secondary Chat** oder **Ausblenden**) jeweils dazugeschrieben. Letztlich bleibt die Entscheidung aber natürlich dir überlassen.

Viel Erfolg!

### Private Nachrichten

**Eingehende Nachrichten:**\
_Empfohlen: Secondary Chat_\
**Beinhaltet:**\
<kbd>-> mir]</kbd>\
**Beinhaltet nicht:**\
<kbd>\[Greeting], », @</kbd>

**Ausgehende Nachrichten:**\
_Empfohlen: Secondary Chat_\
**Beinhaltet:**\
<kbd>\[mir -></kbd>\
**Beinhaltet nicht:**\
<kbd>\[Greeting], », @</kbd>

### Geld

**Eingehende Zahlung:**\
_Empfohlen: Secondary Chat_\
**Beinhaltet:**\
<kbd>gegeben.</kbd>\
**Beinhaltet nicht:**\
<kbd>\[Greeting], @, », ->, :, Du hast</kbd>

**Ausgehende Zahlung:**\
_Empfohlen: Secondary Chat_\
**Beinhaltet:**\
<kbd>gegeben.</kbd>\
**Beinhaltet nicht:**\
<kbd>\[Greeting], @, », ->, :, \[GrieferGames], hat dir</kbd>

**Bank:**\
_Empfohlen: Secondary Chat_\
**Beinhaltet:**\
<kbd>\[Bank]</kbd>\
**Beinhaltet nicht:**\
<kbd>\[Greeting], », ┃</kbd>

**Geld von Kisten / Drops / Server:**\
_Empfohlen: Secondary Chat_\
**Beinhaltet:**\
<kbd>wurden zu deinem Konto hinzugefügt.</kbd>\
**Beinhaltet nicht:**\
<kbd>\[Greeting], »</kbd>

### Allgemeiner Chat

**Plot-Chat:**\
_Empfohlen: Secondary Chat_\
**Beinhaltet:**\
<kbd>\[Plot-Chat]</kbd>\
**Beinhaltet nicht:**\
<kbd>\[Greeting], @, »</kbd>

**Globalchat:**\
**Beinhaltet:**\
<kbd>\[@</kbd>\
**Beinhaltet nicht:**\
<kbd>Leer lassen</kbd>\
**Raum (wenn verfügbar):**\
<kbd>GG-Global</kbd>

**Home-Punkte:**\
_Empfohlen: Secondary Chat_\
**Beinhaltet:**\
<kbd>\[GrieferGames] Deine Home-Punkte:</kbd>\
**Beinhaltet nicht:**\
<kbd>\[Greeting], @, », ┃</kbd>

**Zauberer:**\
_Empfohlen: Secondary Chat_\
**Beinhaltet:**\
<kbd>\[GrieferGames] Ein Zauberer ist auf dem Grundstück</kbd>\
**Beinhaltet nicht:**\
<kbd>\[Greeting], », ┃</kbd>

**CaseOpening:**\
**Beinhaltet:**\
<kbd>\[CaseOpening]</kbd>\
**Beinhaltet nicht:**\
<kbd>\[Greeting], », @</kbd>

**Orbs:**\
_Empfohlen: Secondary Chat_\
**Beinhaltet:**\
<kbd>\[Orbs]</kbd>\
**Beinhaltet nicht:**\
<kbd>\[Greeting], »</kbd>

**Tageszeit wiederhergestellt:**\
_Empfohlen: Ausblenden_\
**Beinhaltet:**\
<kbd>\[GrieferGames] Deine Tageszeit wurde wiederhergestellt.</kbd>\
**Beinhaltet nicht:**\
<kbd>\[Greeting], »</kbd>

**Tageszeit aktualisiert:**\
_Empfohlen: Ausblenden_\
**Beinhaltet:**\
<kbd>\[GrieferGames] Deine Tageszeit wurde vom Grundstück aktualisiert.</kbd>\
**Beinhaltet nicht:**\
<kbd>\[Greeting], »</kbd>

**MobRemover:**\
**Beinhaltet:**\
<kbd>\[MobRemover]</kbd>\
**Beinhaltet nicht:**\
<kbd>», ->, :</kbd>

**Clearlag Time:**\
**Beinhaltet:**\
<kbd>\[GrieferGames] Warnung! Die auf dem Boden liegenden Items werden in</kbd>\
**Beinhaltet nicht:**\
<kbd>», ->, :</kbd>

**Clearlag Item:**\
**Beinhaltet:**\
<kbd>auf dem Boden liegende Items entfernt!</kbd>\
**Beinhaltet nicht:**\
<kbd>», ->, :</kbd>

**AH Überboten:**\
_Empfohlen: Secondary Chat_\
**Beinhaltet:**\
<kbd>\[GrieferGames] Du wurdest bei der Auktion für</kbd>\
**Beinhaltet nicht:**\
<kbd>», ┃</kbd>

**AH Gewonnen:**\
_Empfohlen: Secondary Chat_\
**Beinhaltet:**\
<kbd>\[GrieferGames] Du hast die Auktion für</kbd>\
**Beinhaltet nicht:**\
<kbd>», ┃</kbd>

### Block des Tages

**Eingehende Nachrichten:**\
_Empfohlen: Secondary Chat_\
_Empfohlen: Sound on: random.anvil\_break_\
**Beinhaltet:**\
<kbd>\[Block des Tages]</kbd>\
**Beinhaltet nicht:**\
<kbd>\[Greeting], », ┃, @</kbd>

### Advancements

**Eingehende Nachrichten:**\
_Empfohlen: Secondary Chat_\
**Beinhaltet:**\
<kbd>\[Advancements]</kbd>\
**Beinhaltet nicht:**\
<kbd>\[Greeting], », ┃, @</kbd>

### GrieferGames Pass

**Eingehende Nachrichten:**\
_Empfohlen: Secondary Chat_\
**Beinhaltet:**\
<kbd>\[GrieferPass]</kbd>\
**Beinhaltet nicht:**\
<kbd>\[Greeting], », ┃, @</kbd>
