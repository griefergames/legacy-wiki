---
description: Das erweiterte Trichter-System und seine Funktionen
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

# 📥 Das Trichter-System

Auf GrieferGames wurden die Funktionen der Trichter erweitert. Damit entstehen viele neue Möglichkeiten und auch Verbesserungen.

## Allgemeine Trichter-Informationen

Auf GrieferGames wurden die Trichter-Ticks angepasst, um den Performance-Verbrauch von Trichtern zu reduzieren.&#x20;

### Trichter-Tick

Die Häufigkeit mit der die Trichter auf GrieferGames ticken ist reduziert.&#x20;

Ein Trichter tickt im Standard alle <mark style="color:red;">**8 Ticks**</mark> und verschiebt dabei <mark style="color:red;">**1 Item**</mark>. Auf GrieferGames Tickt ein Trichter alle <mark style="color:green;">**80 Ticks**</mark> und verschiebt dabei <mark style="color:green;">**12 Items**</mark>. Wird in einem Tick kein Item Verschoben, wartet der Trichter ebenfalls 80 Ticks bevor er erneut prüft, ob ein neues Item vorhanden ist.

## Die neuen Trichter-Funktionen

Klickt man beim Schleichen mit Rechtsklick auf einen platzierten Trichter, öffnet sich ein Einstellungsmenü für diesen Trichter.

<figure><img src="../.gitbook/assets/image (13) (1).png" alt=""><figcaption><p>GUI der Trichter-Einstellungen</p></figcaption></figure>

Dieses Menü bietet verschiedene Einstellungsoptionen, welche im Folgenden erläutert werden.

### Item-Anzahl einstellen

Mit dem Button <img src="../.gitbook/assets/image (14) (1).png" alt="" data-size="line"> kann die <mark style="color:orange;">Anzahl der transportierten Items</mark> festgelegt werden.\
Die Standardeinstellung liegt hier bei 12 Items.

Folgende Optionen stehen dir zur Auswahl:

* 1 Item
* 12 Items
* 64 Items

{% hint style="info" %}
Es wird immer nur ein Stack gleichzeitig bewegt. Hat ein Stack weniger Items, als die eingestellte Anzahl, wird nur die Anzahl dieses Stacks verschoben.
{% endhint %}

### Fast Tick

Mit der <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FNT48AEl3AIaqUVOaVIQm%2Fimage.png?alt=media&#x26;token=adafb11e-0799-4974-80bf-fe1b4f91091d" alt="" data-size="line"> <mark style="color:orange;">Fast Tick</mark>-Option ist es möglich, die Tick-Geschwindigkeit auf den Standard zurück zu setzen (siehe [Trichter-Tick](das-trichter-system.md#trichter-tick)). Diese Möglichkeit wird für manche Redstone-Schaltungen benötigt, welche sich nicht anders realisieren lassen. Der Großteil aller Schaltungen lässt sich durch die angepassten Item-Mengen so umbauen, dass diese auch auf GrieferGames funktionieren.

{% hint style="warning" %}
Diese Option steht nur zur Verfügung, wenn sie durch die Administration per `hopper-fast-tick`-Flag auf dem Grundstück freigeschaltet wurde. Diese Flag wird nur in Ausnahmefällen vergeben und kann über das Ticket-System beantragt werden.
{% endhint %}

### Sammelradius

Über die Einstellungsoptionen <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2Fzczdqj57dTuFhUVkkL0t%2Fimage.png?alt=media&#x26;token=d9c251f3-5d06-4c01-8f54-51863107dd10" alt="" data-size="line"> kann der Sammelradius eingestellt werden. Der Sammelradius beeinflusst den Umkreis aus dem ein herumliegendes Item von dem Trichter eingesammelt wird.

Der maximale Sammelradius beträgt <mark style="color:orange;">**15 Blöcke**</mark> und wird außerdem an der <mark style="color:orange;">**Plot-Grenze**</mark> gestoppt.

### Verbundener Trichter

Über die <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FI77II5p9u5a2Nb5f0BDi%2Fimage.png?alt=media&#x26;token=3ca84150-9a43-4a8e-a26c-c76abe38e599" alt="" data-size="line"> <mark style="color:orange;">**Trichter Verbindung**</mark> kann das Ziel des Trichters direkt ausgewählt werden. Das Ziel kann sich in einem Bereich von <mark style="color:orange;">**30 Blöcken**</mark> gewählt werden.

{% hint style="info" %}
Trichter können mit allen Blöcken verbunden werden, welche ein Inventar haben. Die Verbindung ist daher mit allen Blöcken möglich, in die ein Trichter auch standardmäßig weiterleiten kann.
{% endhint %}

Um einen Trichter zu verbinden, klicke auf <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FI77II5p9u5a2Nb5f0BDi%2Fimage.png?alt=media&#x26;token=3ca84150-9a43-4a8e-a26c-c76abe38e599" alt="" data-size="line"> und anschließend mit leerer Hand per Rechtsklick auf den Block, welcher verbunden werden soll.

Beim Klick auf den selben Trichter oder wenn die Entfernung zu groß ist, wird der Verbindungs-Modus beendet.

### Mehrfach-Verbindungen

Über die <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2F7LDPyrR5ayc8CfZYM8Wu%2Fimage.png?alt=media&#x26;token=343b1a56-12e2-44d1-a560-451f6b5b64fb" alt="" data-size="line"> <mark style="color:orange;">**Mehrfachverbindungen**</mark> können mehrere Endpunkte anhand von Materialien für den Trichter festgelegt werden.

#### Übersicht über bestehende Verbindungen

<figure><img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FicHXUR93eIgzXXMxz5V3%2Fimage.png?alt=media&#x26;token=a081d4cf-c35e-4e01-89b3-34ee5d2b1083" alt=""><figcaption><p>Übersichtsseite</p></figcaption></figure>

In dieser Ansicht sind die bereits eingerichteten Verbindungen zu sehen. Pro Material kann immer nur ein Endpunkt als Ziel existieren. Mit einem Klick auf das Material, kann der Endpunkt entfernt werden.

Mit einem Klick auf <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2F70pS79LvC5KqG0ZtwynN%2Fimage.png?alt=media&#x26;token=d9eeba9c-6d3d-4056-98f6-a9e8235f2557" alt="" data-size="line"> <mark style="color:orange;">**Verbindungsmodus starten**</mark> kann der Verbindungsmodus für Multi-Verbindungen gestartet werden.

### Endpunkte hinzufügen / Verbindungs-Modus

Sobald der Verbindungs-Modus aktiv ist, können neue Verbindungen hinzugefügt werden, indem man mit dem gewünschten Material in der Hand auf einen möglichen Endpunkt (siehe Verbundener Trichter) klickt.&#x20;

Die Verbindung wird hinzugefügt, was ebenfalls im Chat bestätigt wird und das nächste Material kann hinterlegt werden.

Der Verbindungs-Modus wird durch Schleichen beendet.

### Optische Anzeige

Mit einem Klick auf <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FpeYcGhMJHH8ouWF2EWS9%2Fimage.png?alt=media&#x26;token=9dfb5f83-0709-4098-9d6d-d67210ffe7c8" alt="" data-size="line"> <mark style="color:orange;">**Optische Anzeige**</mark> werden die Verbindungen und der Sammelradius des Trichters mit farbigen Partikeln angezeigt.&#x20;

* Der Radius wird durch aufsteigende lila Partikel markiert.
* Verbindungen durch statische rote Partikel zwischen Trichter und Endpunkt.

<figure><img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FpjnXFQUFwNDHfr0bpVUe%2Fimage.png?alt=media&#x26;token=b0b59347-8389-488e-9dbf-f1e292417db5" alt=""><figcaption><p>Optische Anzeige</p></figcaption></figure>

### Item-Filter

Mit dem Trichter-System ist es ebenfalls möglich, Items zu filtern, welche in den Trichter aufgenommen werden sollen.

{% hint style="info" %}
Die Filter bestimmen, welche Items ein Trichter "einsaugt" oder aus anderen Inventaren entnimmt. Legt man Items direkt in den Trichter, werden die Filter nicht berücksichtigt.
{% endhint %}

Die Filter-Optionen lassen sich ebenfalls miteinander kombinieren.

Die Filter können mit einem Shift-Klick auf das <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FUUIhQ2kdINw7HfrQjTUm%2Fimage.png?alt=media&#x26;token=cb5c4ce8-3189-4451-b1ab-4a337d90526d" alt="" data-size="line"> Filter-Icon entfernt werden. Das Icon wechselt je nach gefiltertem Material.

#### Material-Filter

<figure><img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2Fi8MU83m4w5URf77yH1Ww%2Fimage.png?alt=media&#x26;token=95fdbac3-5ac8-4960-8fe9-27e1412cb39a" alt=""><figcaption><p>Beispiel Material-Filter auf Grasblock</p></figcaption></figure>

Um ein Material für den Trichter zu filtern, kann das Material im Hauptmenü aus dem eigenen Inventar ausgewählt werden. Das gefilterte Material ist dann an der Stelle des <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FUUIhQ2kdINw7HfrQjTUm%2Fimage.png?alt=media&#x26;token=cb5c4ce8-3189-4451-b1ab-4a337d90526d" alt="" data-size="line"> zu sehen.

Mit dem Klick auf das gefilterte Material oder <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FUUIhQ2kdINw7HfrQjTUm%2Fimage.png?alt=media&#x26;token=cb5c4ce8-3189-4451-b1ab-4a337d90526d" alt="" data-size="line"> öffnet sich das Filter-Menü mit den folgenden Optionen:

<figure><img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FTHLaAd38BrkGEtBUqX3e%2Fimage.png?alt=media&#x26;token=4baadaf5-09e2-4386-a45c-9579f5b8d293" alt=""><figcaption><p>Filter-Übersicht</p></figcaption></figure>

#### Verzauberungs-Filter

Mit einem Klick auf den <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FyjfK1PHbthxuu0Sp5xpl%2Fimage.png?alt=media&#x26;token=6019f8a4-eff7-4829-9136-b79c011de270" alt="" data-size="line"> <mark style="color:orange;">**Verzauberungs-Filter**</mark> aktiviert sich der Verzauberungsfilter. Bei einem weiteren Klick öffnet sich das Menü mit den filterbaren Verzauberungen.

<figure><img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FOvpxp5u7drdDHj78KqE1%2Fimage.png?alt=media&#x26;token=bb92ec13-fed0-43a7-8b09-05e2f0b78632" alt=""><figcaption><p>Übersichtsseite Verzauberungen</p></figcaption></figure>

In dieser Ansicht können nun die Verzauberungen angewählt werden, welche auf dem Item vorhanden sein müssen. Mit **Rechtsklick** wird die gewünschte Verzauberungsstufe erhöht, mit einem **Linksklickt** verringert. Mit einem **Shift-Klick** wird die Verzauberung aus dem Filter entfernt.

{% hint style="warning" %}
Werden mehrere Verzauberungen gewählt, müssen alle Verzauberungen auf dem Item vorhanden sein. Es muss auch die entsprechende Stufe der Verzauberung vorhanden sein.
{% endhint %}

Zusätzlich zu dem Verzauberungsfilter steht mit dem <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FUUIhQ2kdINw7HfrQjTUm%2Fimage.png?alt=media&#x26;token=cb5c4ce8-3189-4451-b1ab-4a337d90526d" alt="" data-size="line"> unter dem <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FyjfK1PHbthxuu0Sp5xpl%2Fimage.png?alt=media&#x26;token=6019f8a4-eff7-4829-9136-b79c011de270" alt="" data-size="line"> der Filter "keine Verzauberung" zur Verfügung.

#### Signierungs-Filter

Mit einem Klick auf den <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FgVfl6sMpdCcChYQtD8Nw%2Fimage.png?alt=media&#x26;token=8684d650-c99b-4f9b-a859-afcdc5658f3f" alt="" data-size="line"> <mark style="color:orange;">**Signierungs-Filter**</mark> aktiviert sich der Signierungsfilter. Bei einem weiteren Klick öffnet sich das Menü für die Einstellung der Signierung.

<figure><img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2F3f97A6lZaRhM7y9MJzBO%2Fimage.png?alt=media&#x26;token=d7c8d494-e29c-46bf-ab9c-6d6f8f24607e" alt=""><figcaption><p>Einstellungsmenü Signierung</p></figcaption></figure>

Die folgenden Optionen der Signierung können eingestellt werden:

* <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2Fx0uuH8M9M9f1GyDdm80u%2Fimage.png?alt=media&#x26;token=e7b11d06-5e70-42f8-a080-62d5105e8da3" alt="" data-size="line">**Signierung von:** Filtert welcher Spieler die Signierung erstellt haben muss
* <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FJyHqV1CfzOgaRi5tx6OK%2Fimage.png?alt=media&#x26;token=25207249-f709-41ae-8b93-e436d0eaf8c8" alt="" data-size="line">**Signierung am:** Filtert an welchem Datum die Signierung erstellt wurde
* <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FIJXE0XEx96w2EczqxbSe%2Fimage.png?alt=media&#x26;token=d6c6f69a-e6d0-4662-baa2-363b8eed3308" alt="" data-size="line">**Signierung:** Filtert den Text der Signierung

{% hint style="info" %}
Der Text der Signierung muss die eingestellten Zeichen / den eingestellten Text nur enthalten und nicht vollständig entsprechen.
{% endhint %}

#### Beschreibungs-Filter

Mit einem Klick auf den <img src="https://1446237620-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fi10PgHQTIUUm2awhkL0L%2Fuploads%2FIJXE0XEx96w2EczqxbSe%2Fimage.png?alt=media&#x26;token=d6c6f69a-e6d0-4662-baa2-363b8eed3308" alt="" data-size="line"> <mark style="color:orange;">**Beschreibungs-Filter**</mark> aktiviert sich der Beschreibungs-Filter. Bei einem weiteren Klick öffnet sich das Menü zum Hinzufügen von Beschreibungen.

<figure><img src="../.gitbook/assets/image (15) (1).png" alt=""><figcaption><p>Beschreibungsfilter-Menü</p></figcaption></figure>

Mit dem Button <img src="../.gitbook/assets/image (17) (1).png" alt="" data-size="line"> kannst du eine neue Beschreibung als Filter-Option hinzufügen.\
Im nachfolgenden Amboss-Menü kannst du den Text, welcher gefiltert werden soll, eintragen und per Klick auf das fertige Produkt bestätigen. Dein ausgewählter Filter wird im Menü angezeigt. Es können auch mehrere Filter hinterlegt werden.

<figure><img src="../.gitbook/assets/image (18) (1).png" alt=""><figcaption><p>Beschreibungsfilter-Menü mit 2 Einträgen</p></figcaption></figure>

* Durch einen Klick auf einen hinzugefügten Beschreibungsfilter kannst du diesen bearbeiten.
* Durch Umschalt+Klick auf einen Beschreibungsfilter kannst du diesen komplett löschen.

#### Namens-Filter

Mit einem Klick auf den <img src="../.gitbook/assets/image (19) (1).png" alt="" data-size="line"> <mark style="color:orange;">**Namens-Filter**</mark> aktivierst du die Filterung nach umbenannten Items. In der Standard-Einstellung werden alle umbenannten Items gefiltert. Bei einem weiteren Klick öffnet sich ein Amboss-Menü, in welchem du einen bestimmten Namen festlegen kannst. Durch Klick auf das fertige Produkt übernimmst du diesen.

* Durch das Entfernen des Eintrags im Amboss-Menü vor dem Bestätigen wird wieder der Standard-Filter für alle umbenannten Items aktiviert.
* Durch Umschalt-Klick auf den Namens-Filter deaktiviert sich der Namens-Filter vollständig.



<details>

<summary>An diesem Artikel beteiligt</summary>

* [50U7R34P3R](https://profile.griefergames.live/minecraft/8e2ce0be-aa2c-46a7-a2dc-48f948743edf)

</details>
