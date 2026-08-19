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
    visible: true
  tags:
    visible: true
  actions:
    visible: true
---

# Grundstücksrechte vergeben

### Helfer hinzufügen

Grundstücks-Helfer können auf deinem Grundstück bauen (Blöcke setzen, abbauen & interagieren), solange du auf dem jeweiligen Citybuild-Server online bist. Diese Spieler haben keinen Zugriff auf die Grundstück-Einstellungen.&#x20;

Der Befehl lautet: `/p add <Spielername>`

### Vertrauten hinzufügen

Grundstück-Vertraute können jederzeit auf deinem Grundstück bauen (Blöcke setzen, abbauen & interagieren). Diese Spieler haben keinen Zugriff auf die Grundstück-Einstellungen.

Der Befehl lautet: `/p trust <Spielername>`

### Besitzer ändern

Du kannst die kompletten Rechte für das Grundstück an einen anderen Spieler übergeben. Du bist danach nicht mehr der Eigentümer des Grundstücks. Diese Methode wird beispielsweise verwendet, um ein Grundstück zu verkaufen.

Der Befehl lautet: `/setowner <Spielername>`

Anschließend bestätigen beide Spieler, dass die kompletten Grundstücksrechte übertragen werden sollen.

Der Befehl lautet: `/setowner confirm`

{% hint style="warning" %}
Geh vorsichtig mit dem Vergeben von Rechten um und gebe sie nur an Leute, denen du vertraust.
{% endhint %}

### Rechte entfernen

Du kannst die Rechte eines Spielers auch jederzeit wieder entfernen.

Der Befehl lautet: `/p remove <Spielername>`

### Zutritt verweigern

Nach Ausführung des Befehls kann der angegebene Spieler das Grundstück nicht mehr betreten.

Der Befehl lautet: `/p deny <Spielername>` oder `/p deny *`

Mit `*` wird **jeder** Spieler von deinem Grundstück ausgeschlossen – Spieler, die Baurechte haben, können weiterhin das Grundstück betreten.

### Zutritt zulassen

Ein Spieler war vom Grundstück ausgeschlossen und soll es wieder betreten können?

Der Befehl lautet: `/p undeny <Spielername>` oder `/p undeny *`

Hierbei gilt das Selbe, wie beim Ausschließen mit `*` – es erhält wieder jeder Spieler Zutritt zum Grundstück.

{% hint style="warning" %}
Der Befehl `/p undeny` ist ein Alias für den Befehl `/p remove`.

Wenn Helfer oder Vertraute gesetzt sind, werden diese daher beim "Freigeben" ebenfalls wieder zurückgesetzt. Der Befehl muss dann mehrfach wiederholt werden, um die einzelnen Kategorien (Helfer, Vertraute, Verboten) nacheinander zurückzusetzen.
{% endhint %}
