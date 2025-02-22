# Spawner, Hologramme & Partikeleffekte verwalten

### Ich möchte einen Spawner verschieben lassen.

Spawner kannst du ohne den Verlust des Items nicht abbauen.

Auch von Administratoren werden Spawner grundsätzlich nicht umgesetzt, da dies unter die Erstattung von Items fällt, was auf GrieferGames generell nicht gemacht wird. Jedoch besteht trotzdem die Möglichkeit, dass der Spawner umgesetzt wird, wenn du einen Admin entweder in Minecraft oder auf dem TeamSpeak-Server nett fragst, wobei das Spammen hier nicht zum Erfolg führt. \
Alternativ kannst du auch Teammitglieder mit administrativen Rechten, die auf GrieferGames livestreamen, fragen.

Dazu gesagt gibt es auch keine Möglichkeit, mit einer höheren Behutsamkeit-Verzauberung auf einer Spitzhacke einen Spawner abzubauen.



### Das Hologramm wurde nicht entfernt.

Ein Spieler hat ein Hologramm auf einem Grundstück hinterlassen, welches du erhalten hast?

Normalerweise sollte unser Plugin spätestens nach dem nächsten Server-Neustart (täglich 04:00 Uhr) das Hologramm automatisch gelöscht haben, da es erkennt, dass der Hologramm-Besitzer nicht mehr mit dem Grundstücksbesitzer übereinstimmt.

Wenn dies nicht der Fall ist, kannst du mit dem Befehl `/pholo removeplot` [alle Hologramme auf dem Grundstück löschen](../../grundlagen/befehlsuebersicht/spezielle-features/hologramme.md). Eigene Hologramme kannst du nachfolgend selbst wieder hinzufügen.

Sollte sich ein Hologramm mit dem Befehl nicht entfernen lassen, wende dich bitte an einen Supporter/Moderator.



### Ich möchte einen Partikeleffekt löschen.

Zum Löschen eines Partikeleffektes ist es zunächst wichtig, dass du dich in einem geringen Umkreis zu diesem befindest (rund 5 Blöcke). Bei einem zu großen Abstand ist das Löschen gegebenenfalls nicht möglich.&#x20;

Zuerst gilt es, über `/removeparticle` alle aktiven Partikeleffekte in deinem Umfeld anzeigen zu lassen. Im folgenden Screenshot ist nur ein Partikel in der Nähe platziert:

<figure><img src="../../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Anzeige eines Partikels nach Ausführung des Befehls <code>/removeparticle</code></p></figcaption></figure>

Bei mehreren Partikeleffekten in deinem näheren Umkreis kannst du üblicherweise die genaue Position (X-, Y- & Z-Koordinaten) und Partikelart (bspw. **Beam** oder **Helix**) ermitteln, damit du den richtigen Effekt löschst. Ist der zu löschende Effekt ersichtlich, verwendest du die im Chat angegebene Nummer zum Löschen.&#x20;

Für unser oberes Beispiel ist dies die Nummer **1.** Du gibst nun an, dass der Partikeleffekt 1 gelöscht werden soll. \
Der Befehl lautet daher: `/removeparticle 1`.

Als letzten Schritt musst du die Löschung bestätigen. Mit dem Bestätigen wird der Effekt gelöscht. Das Partikel-Item wird dabei nicht zurück erstattet. Zur Bestätigung der Löschung verbleiben 60 Sekunden.

Der Befehl lautet: `/removeparticle confirm`&#x20;

<figure><img src="../../.gitbook/assets/image (2) (1).png" alt=""><figcaption><p>Anzeige nach erfolgreicher Löschung des Partikels</p></figcaption></figure>



<details>

<summary>An diesem Artikel beteiligt</summary>

* [50U7R34P3R](https://profile.griefergames.live/minecraft/8e2ce0be-aa2c-46a7-a2dc-48f948743edf)

</details>
