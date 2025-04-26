---
description: Der (fast) unbegrenzte Speicher auf GrieferGames
---

# 📦 Das Unendliche Lager

Die [unendlichen Lager](https://wiki.griefergames.live/funktionen/features/unbegrenzter-speicher) stehen euch nun ebenfalls auch auf dem 1.8 Netzwerk zur Verfügung. Hier allerdings in etwas abgewandelter Form mit mehreren Besonderheiten.

<details>

<summary>Folgende Items sind lagerbar:</summary>

* Karotten
* Kartoffeln
* Zuckerrohr
* Pilze
* Kakteen
* Weizen
* Samen
* Melonenscheiben&#x20;
* Kürbisse
* Diamant
* Smaragd
* Lapis
* Kohle
* Redstone
* Eisenbarren
* Goldbarren
* Goldklumpen
* Bruchstein
* Bemosster Bruchstein
* Erde
* Stein
* Pfeil
* Hasenpfote
* Kaninchenfell
* Leder
* Federn
* Prismarinscherben
* Prismarinkristalle
* Zucker
* Spinnenauge
* Glowstonestaub
* Stock
* Schwarzpulver
* Glasflasche
* Magmacreme
* Lohenrute
* Faden
* Enderperle
* Verrottetes Fleisch
* Ghast-Träne
* Schleimball
* Knochen
* Tintenbeutel
* Rohes Rindfleisch
* Rohes Hühnchen
* Rohes Kaninchen
* Rohes Hammelfleisch
* Roher Fisch
* Eier
* Netherwarze
* Sonnenblume
* Melonenblock
* Grasblock
* Sand
* Sandstein
* XP-Flaschen
* Schneeball
* Schneeblock
* Eis
* Packeis
* Spinnennetz
* Seerosenblatt
* Netherquarzerz
* Rosenstrauch
* Flieder
* Pfingstrose
* Lohenstaub
* Feuerkugel
* Enderauge
* Ranken
* Myzel
* Kies
* Feuerstein
* Seelaterne
* TNT
* Amboss
* Bücher
* Schüssel
* Leerer Eimer
* Papier
* Kompass
* Leere Karte
* Ofen
* Plattenspieler
* Braustand
* Zaubertisch
* Endertruhe
* Rahmen
* Kessel
* SChild
* Eisengitter
* Gemälde
* Leine
* Uhr
* Werkbank
* Steinziegel
* Ziegelsteine
* Ziegel
* Netherziegel
* Schleimblock
* Ofenkartoffel
* Schwamm
* Fermentiertes Spinnenauge
* Goldene Karotte
* Rüstungsständer
* Glitzernde Melonenscheibe
* Wolle (alle Farben)
* Gras (alle Arten)
* Blumen (alle Arten)
* Erze (alle Arten)
* Erzblöcke (alle Arten)
* Holzstamm (alle Arten)
* Holzbrett (alle Arten)
* Ton (alle Arten)
* Teppiche (alle Arten)
* Nether-Blöcke (alle Arten)
* Glas (alle Arten)
* Laub (Alle Arten)
* Pilzblock (Alle Arten)
* Prismarinblock (Alle Arten)
* Redstone-Items (Alle Arten)

Alle Sub-ID's dieser Items (bspw. Granit bei Stein oder div. Farben bei Wolle) sind hierin mit einbegriffen.

</details>

### Crafting-Rezept

Das unendliche Lager kann über folgendes Rezept in der Werkbank hergestellt werden:

<figure><img src="https://lh7-us.googleusercontent.com/docsz/AD_4nXd_tdVEkQ9mSuj0oYU_3nZoSfVi9slk0L9wIH30Htzts7UBNnF3ErlSzgPTRPx3W7USVVlUddkwzfQJyKIkRpq6WjgHg01iHR8Rs4Ce4vvORoAuvQ0-Vg0WzhcHwal3BBIaSuTmuFYvixkUDlD70npfU-Vw?key=Fbef1cizwBxjBjyjDaG3uQ" alt=""><figcaption><p>Herstellungsrezept des Unendlichen Lagers auf dem 1.8-Netzwerk</p></figcaption></figure>



### Allgemeine Funktionsweise

Anders als auf der Cloud ist das [unendliche Lager auf der 1.8 eine Truhe](https://items.griefergames.net/#Unbegrenzter_Speicher) und speichert weit aus mehr Items (also über 2.147.483.647 Einheiten).&#x20;

Das Lager speichert immer den Item-Typ, welcher als erstes reingelegt wurde - ab diesem Zeitpunkt ist das Lager speziell auf dieses Item fixiert und kann keine anderen Items mehr aufnehmen. Pro Grundstück können zwar mehrere unendliche Lager eines bestimmten Item-Typs verwendet werden, allerdings kann nur eines davon als ["passive Farm" (Einsaugmodus)](das-unendliche-lager.md#passive-farmen)​​ aktiv sein.&#x20;

Außerdem sind auch Verbindungen mit Trichtern möglich. Die Funktionen des [Trichter-Systems](das-trichter-system.md) können also auch auf ein Unendliches Lager geleitet werden.

Die Lager lassen sich nur abbauen, wenn sie komplett leer sind. Durch `/breakblock` ist das Abbauen auch in gefülltem Zustand möglich. Die Items gehen in diesem Fall verloren.

Unendliche Lager lassen sich mit der Flag `/unlimited-storage-public` für andere Spieler auf einem Grundstück freigeben.



### Komprimierte Items

Das unendliche Lager verfügt außerdem über einen automatischen Komprimierer. Das bedeutet, dass man mit Shift + Rechtsklick auf die Kiste in ein Menü kommt, aus welchem man sich das gelagerte Item direkt [in komprimierter Form](../erweiterte-features/die-rezeptsammlung.md#item-komprimierung) rausziehen kann.

<figure><img src="https://lh7-us.googleusercontent.com/docsz/AD_4nXceDepXC_XNRdYYalRHWNtwTzsVQ5ko1AwrZv1g3ebCPUrN-5xBV7HszMGzJXisuczfKh1Hyi-1rTSVZhG05KdFJx1zLViiUqndY3bEM7-v5C9J-V8duIT5fa-RHNt0DKFc7sBcbURg4iEz7q7o82DSV_ZD?key=Fbef1cizwBxjBjyjDaG3uQ" alt=""><figcaption><p>Abruf eingelagerter Items mit vorher eingestellter Komprimierungsstufe</p></figcaption></figure>



### Passive Farmen

Über Shift + Rechtsklick hat man außerdem auch die Möglichkeit, die "passive Farm" (Einsaug-Modus) des Unendlichen Lagers zu aktivieren.&#x20;

Nach Auswahl werden alle Items dieses Typs, die auf dem Grundstück natürlich entstehen oder gedroppt werden würden, automatisch direkt in das Lager geleitet. \
Diese Funktion greift priorisiert vor dem "Einsaugen" durch Trichter.



### Einsaug-Modus zurücksetzen

Um den Einsaug-Modus zurückzusetzen, kann man diesen am jeweiligen Unendlichen Lager wieder ausschalten. \
Falls ein Unendliches Lager/Einsaug-Modus fehlerhaft hinterlegt ist, kann über den Befehl `/storage clear` der Fehler selbstständig behoben werden. Über den Befehl werden **alle** aktiven Einsaug-Modi auf dem jeweiligen Grundstück aufgehoben. \
Die Einsaug-Modi können dann an den Unendlichen Lagern neu eingestellt werden.\




<details>

<summary>An diesem Artikel beteiligt</summary>

* [SyntaxOfficial](https://profile.griefergames.live/minecraft/5680a974-0d5f-460d-87a2-a33b076d4d08)
* [50U7R34P3R](https://profile.griefergames.live/minecraft/8e2ce0be-aa2c-46a7-a2dc-48f948743edf)

</details>
