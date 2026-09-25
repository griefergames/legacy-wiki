---
description: >-
  /createkarte wurde mit den Winterkisten 2024 (04.12.2024) eingeführt. Wie
  funktioniert das Feature?
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: false
  pagination:
    visible: true
  metadata:
    visible: true
  tags:
    visible: true
  actions:
    visible: true
  anchors:
    visible: true
---

# 🗺️ Karten

Motivkarten zu bauen braucht Zeit, Material und eine Menge Erfahrung.

Wäre es da nicht schön, sein Wunschmotiv schnell und einfach als Karte verfügbar zu haben und sein Heim damit zu dekorieren? Hier hilft der Kartengenerator!

Wer seine Karte lieber selbst Block für Block baut, findet im Tutorial [Vom Bild zur Karte](../tutorials/vom-bild-zur-karte.md) eine ausführliche Anleitung.

### Das Recht

Um den Kartengenerator nutzen zu können, benötigt man das entsprechende [Recht](https://items.griefergames.net/#Rechte_%7C_%2Fcreatekarte-Recht).

{% hint style="danger" %}
Derzeit ist dieses Recht nur begrenzt verfügbar.
{% endhint %}

Hat man das Recht eingelöst, erhält man die Berechtigung, den Befehl `/createkarte` zu verwenden.

### Was geht, was nicht?

Der Kartengenerator hat einige Einschränkungen:

* Der Befehl hat einen Cooldown von 7 Tagen.
* Die erstellten Karten haben ein AntiCopy vom Server (lässt sich nicht entfernen).
* Die maximale Kartengröße beträgt 36 Teile und die Karte muss rechteckig sein.
  * Die Karte kann auch eine kleinere Größe haben und somit aus weniger Teilen bestehen. Dies ermöglicht auch die Erstellung von Karten im Format 3x4 oder 4x4.
  * 36 Kartenteile sind auch in anderer Anordnung möglich, solange die Karte rechteckig ist. Dies ermöglicht beispielsweise auch Karten im Format 3x12, 4x9 oder 6x6.

### Das Motiv vorbereiten

Der Kartengenerator nimmt eine vorgefertigte Grafik (Bilddatei) und wandelt diese in eine Minecraftkarte um.

Damit der korrekte Farbraum und die Kartengröße ermittelt werden können, ist etwas Vorarbeit nötig.

Die Bilddatei muss eine Größe aufweisen, die sich in Höhe und Breite jeweils durch 128 Pixel teilen lässt. 128 Pixel werden für ein Kartenteil benötigt. Eine Grafik für eine Karte mit 6x6 Kartenteilen benötigt also beispielsweise eine Größe von 768 x 768 px. Eine Bilddatei für eine 3x4-Karte hätte eine Größe von 384 x 512 px.

Minecraft beherrscht in der 1.8 nur eine begrenzte Anzahl an Farben. Ist eine Farbe nicht umsetzbar, wird per Annäherung ein entsprechender Farbwert ermittelt. Dies geschieht automatisch und muss nicht vorher in der Bilddatei angepasst werden. Jedoch führt dieser Vorgang zu einem Qualitätsverlust und kann ggf. zu "falschen" Farbwerten in der Karte führen.

### Das Motiv hochladen

Habt ihr eure Bilddatei vorbereitet und auf die korrekte Größe gebracht, müsst ihr diese ins Internet hochladen, um sie für den Generator verfügbar zu machen. Hierfür wird der Dienst ImgBB verwendet.

Ladet das Bild also auf der Seite [https://imgbb.com/](https://imgbb.com/) hoch.

Im nächsten Schritt benötigt ihr den Direktlink zur Grafik. Öffnet hierfür den „Betrachter-Link“, den ihr auf der Seite erhaltet, in einem neuen Tab oder Fenster.

<figure><img src="../../.gitbook/assets/image (135).png" alt=""><figcaption><p>Den Betrachter-Link findet ihr nach dem Hochladen unter „Embed-Codes“.</p></figcaption></figure>

Führt einen Rechtsklick auf das Bild durch und wählt aus, dass das Bild in einem neuen Tab geöffnet wird.

<figure><img src="../../.gitbook/assets/image (136).png" alt=""><figcaption></figcaption></figure>

Führt erneut einen Rechtsklick auf das Bild durch und wählt „Bildadresse kopieren“ aus.

<figure><img src="../../.gitbook/assets/image (137).png" alt=""><figcaption></figcaption></figure>

Der zuletzt abgerufene Link enthält den Direktlink zu dem von euch hochgeladenen Bild und hat eine entsprechende Datei-Endung (`.jpg`, `.png`, `.gif` usw.).

### Die Karte erstellen

Im letzten Schritt könnt ihr die Karte auf unserem Netzwerk erstellen. Gebt hierfür den Befehl `/createkarte <Link>` ein. Den Platzhalter `<Link>` ersetzt ihr dann durch die kopierte Adresse der Bilddatei.

Ihr erhaltet die entsprechenden Karten (je nach Größe des hochgeladenen Motivs) in euer Inventar. Beachtet, dass ihr genügend Platz in Hotbar und Inventar habt, um alle Kartenteile entgegenzunehmen.
