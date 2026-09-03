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

# Spawner, Hologramme & Partikeleffekte verwalten

### Spawner verschieben?

Eine direkte Möglichkeit Spawner zu verschieben gibt es nicht.\
Mit einer Spawner-Spitzhacke können jedoch Spawner auf dem Grundstück abgebaut und erhalten werden. Beim Abbau besteht **eine Chance** darauf, dass der Spawner als Item dropped.&#x20;

{% hint style="info" %}
Die Spawner-Spitzhacke funktioniert nur in der Plotwelt. Die mögliche Drop-Rate des Spawners ist auf der Spitzhacke vermerkt.
{% endhint %}

### Hologramme anderer Spieler

Hat man Hologramme auf dem eigenen Grundstück, welche nicht einem selbst gehören, kann man diese per Befehl entfernen.

Über den Befehl `/pholo removeplot` werden [alle Hologramme auf dem Grundstück](../../grundlagen/befehlsuebersicht/spezielle-features/hologramme.md) gelöscht. Das heißt, dass die eigenen Hologramme eigenständig neu gesetzt werden müssen.&#x20;

Sollte sich ein Hologramm mit dem Befehl nicht entfernen lassen, empfehlen wir, dass man sich bei einem Teammitglied meldet.

### Wie lösche ich einen Partikeleffekt?

Zum Löschen eines Partikeleffektes ist es notwendig, dass man sich in einem geringen Umkreis zu diesem befindest. Ist der Abstand zu groß, wird er dir eventuell nicht in der Übersicht angezeigt.

Über `/removeparticle` kann man alle aktiven Partikeleffekte im näheren Umfeld anzeigen lassen. Im folgenden Screenshot ist nur ein Partikel in der Nähe platziert:

<figure><img src="../../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption><p>Anzeige eines Partikels nach Ausführung des Befehls <code>/removeparticle</code></p></figcaption></figure>

Bei mehreren Partikeleffekten im näheren Umkreis kann man üblicherweise die genaue Position (X-, Y- & Z-Koordinaten) und die Partikelart (bspw. **Beam** oder **Helix**) ermitteln, damit man den richtigen Partikeleffekt löscht. Ist der zu löschende Effekt ersichtlich, verwendet man die im Chat angezeigte Nummer zum Löschen.&#x20;

Für unser oberes Beispiel ist dies die Nummer **1.** Im Chat gibt man daher an, dass der Partikeleffekt 1 gelöscht werden soll.  Der Befehl dafür lautet: `/removeparticle 1`.

Als letzten Schritt ist es notwendig die Löschung zu bestätigen. Mit dem Bestätigen wird der Effekt gelöscht. Das Partikel-Item wird dabei nicht zurück erstattet. Zur Bestätigung der Löschung hat man 60 Sekunden Zeit. Der Befehl lautet: `/removeparticle confirm`&#x20;

<figure><img src="../../.gitbook/assets/image (2) (1).png" alt=""><figcaption><p>Anzeige nach erfolgreicher Löschung des Partikels</p></figcaption></figure>
