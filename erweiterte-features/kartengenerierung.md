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
---

# 🗺️ Kartengenerierung

Motivkarten zu bauen braucht Zeit, Material und eine Menge Erfahrung.&#x20;

Wäre es da nicht schön sein Wunschmotiv schnell und einfach als Karte verfügbar zu haben und sein Heim damit zu dekorieren? Hier hilft der Kartengenerator!

### `/createkarte` - Das Recht

Um den Kartengenerator nutzen zu können, benötigt man das entsprechende [Recht](https://items.griefergames.net/#Rechte_%7C_%2Fcreatekarte-Recht).&#x20;

{% hint style="danger" %}
Derzeit ist dieses Recht nur begrenzt verfügbar und aus den Winter-Kisten erhältlich.
{% endhint %}

Hat man das Recht gewonnen und eingelöst, erhält man die Berechtigung den Befehl `/createkarte` zu verwenden.&#x20;



### `/createkarte` - Was geht, was nicht?

Der Kartengenerator hat einige Einschränkungen.&#x20;

* Der Befehl hat einen Cooldown von 7 Tagen
* Die erstellten Karten haben ein AntiCopy vom Server (lässt sich nicht entfernen).
* Die maximale Kartengröße beträgt 36 Teile und die Karte muss rechteckig sein.
  * Die Karte kann auch eine kleinere Größe haben und somit aus weniger Teilen bestehen.\
    Dies ermöglicht auch die Erstellung von Karten im Format 3x4 oder 4x4.
  * 36 Kartenteile sind auch in anderer Anordnung möglich, solange sie rechteckig ist. \
    Dies ermöglicht beispielsweise auch Karten im Format 3x12, 4x9 oder 6x6.



### `/createkarte` - Das Motiv vorbereiten

Der Kartengenerator nimmt eine vorgefertigte Grafik (Bilddatei) und wandelt diese in eine Minecraftkarte um.&#x20;

Um sicherzustellen, dass der korrekte Farbraum und die Kartengröße ermittelt werden kann, benötigt es hierfür bestimmte Vorarbeit.

Die Bilddatei muss eine Größe aufweisen welche sich in Höhe/Breite jeweils durch 128 Pixel teilen lässt.\
128 Pixel werden für ein Kartenteil benötigt. Eine Grafik für eine Karte mit 6x6 Kartenteilen benötigt also beispielsweise eine Größe von 768 x 768 px. Eine Bilddatei für eine 3x4-Karte wäre 384 x 512 px breit.

Minecraft beherrscht in der 1.8 nur eine begrenzte Anzahl an Farben. Ist eine Farbe nicht umsetzbar wird per Annäherung ein entsprechender Farbwert ermittelt. Dies geschieht automatisch und muss nicht vorher in der Bilddatei angepasst werden. \
Jedoch führt dieser Vorgang zu einem Qualitätsverlust und kann ggf. zu "falschen" Farbwerten in der Karte führen.



### `/createkarte` - Das Motiv hochladen

Habt ihr eure Bilddatei vorbereitet und auf die korrekte Größe gebracht, müsst ihr diese im Internet hochladen, um sie für den Generator verfügbar zu machen. Hierfür wird der Dienst ImgBB vom Anbieter Imgur verwendet.

Die Karte wird von euch also auf der Seite [https://imgbb.com/](https://imgbb.com/) hochgeladen.&#x20;

Im nächsten Schritt benötigt ihr den Direktlink zur Grafik. Öffnet hierfür den "Betrachter-Link", welchen ihr auf der Seite erhaltet in einem neuen Tab/Fenster.

<figure><img src="../.gitbook/assets/image (135).png" alt=""><figcaption></figcaption></figure>

Führt einen Rechtsklick auf das Bild durch und wählt aus, dass das Bild in einem neuen Tab geöffnet wird.

<figure><img src="../.gitbook/assets/image (136).png" alt=""><figcaption></figcaption></figure>

Führt erneut einen Rechtsklick auf das Bild durch und wählt aus, dass ihr die Grafikadresse kopieren wollt.

<figure><img src="../.gitbook/assets/image (137).png" alt=""><figcaption></figcaption></figure>

Der zuletzt abgerufene Link enthält den Direktlink zu dem von euch hochgeladenen Bild und hat eine entsprechende Datei-Endung (`.jpg`, `.png`, `.gif`, etc.)



### `/createkarte` - Die Karte erstellen

Im letzten Schritt könnt ihr die Karte auf unserem Netzwerk erstellen. Gebt hierfür den Befehl `/createkarte <Link>` ein.  Den Platzhalter \<Link> ersetzt ihr dann mit der kopierten Adresse der Bilddatei.

Ihr erhaltet die entsprechenden Karten (je nach Größe des hochgeladenen Motivs) in euer Inventar. Beachtet, dass ihr genügend Platz in Hotbar und Inventar habt, um alle Kartenteile entgegen zu nehmen.



<details>

<summary>An diesem Artikel beteiligt</summary>

* [50U7R34P3R](https://profile.griefergames.live/minecraft/8e2ce0be-aa2c-46a7-a2dc-48f948743edf)

</details>
