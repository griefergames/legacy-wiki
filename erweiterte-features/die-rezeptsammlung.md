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

# 🧾 Die Rezeptsammlung

In der Spielversion 1.8 ist das Rezeptbuch aus den höheren Spiel-Versionen noch nicht vorhanden.&#x20;

Ersatzweise haben wir daher den Befehl `/rezepte` hinzugefügt, mit welchem ihr ein GrieferGames-eigenes Rezeptbuch (Rezeptsammlung) aufrufen könnt.

In der Rezeptsammlung habt ihr 4 verschiedene Auswahlmöglichkeiten:

* [Standardrezepte](die-rezeptsammlung.md#standardrezepte)
* [Item-Komprimierung](die-rezeptsammlung.md#item-komprimierung)
* [Spezial-Rezepte](die-rezeptsammlung.md#spezial-rezepte)
* [CustomBlocks](die-rezeptsammlung.md#customblocks)

### Standardrezepte

Hierbei handelt es sich um eine Sammlung aller Standard-Minecraft-Rezepte. Du kannst hier das passende Item aus den vorhandenen Kategorien heraussuchen. Öffnest du ein Rezept und hast alle benötigten Materialien im Inventar kannst du das Item auch direkt in der Rezept-Ansicht herstellen.

Hast du bereits ein Item im Inventar, von welchem du mehr herstellen willst, so kannst du nach Auswahl der Standard-Rezepte auf das Item in deinem Inventar klicken. Wenn es ein Rezept zur Herstellung gibt, wirst du direkt in die Rezept-Ansicht des Items gebracht.

{% hint style="info" %}
Einige Items haben mehrere verschiedene Rezeptvarianten. Diese können über das +/- Symbol in der Rezeptansicht gewechselt werden.
{% endhint %}

### Item-Komprimierung

Items sind wichtig und je mehr man hat, desto mehr kann man damit machen. Aber irgendwann wird auch das größte Lager voll.

Deswegen gibt es die Item-Komprimierung. Im Sinne von Erzen, welche sich zu Barren verschmelzen lassen haben wir keine Mühen gescheut und eine Vielzahl an Items mit eigenen Rezepten versehen, mit welchen du diese "komprimieren" kannst. Mit diesem Vorgang kannst du mehrere Items zu einem einzigen zusammenfügen, welches diese enthält.&#x20;

Der Vorgang lässt sich auf 7 Stufen herauf wiederholen, sodass du mehrere Millionen Items derselben Art auf einem einzigen Slot haben kannst. Du kannst mit diesen sogar ganz normal bauen oder sie für Interaktionen mit dem [Adventurer](das-adventurer-system.md#abgabe-aufgaben) und dem [Orb-Händler](das-orb-system.md#der-orb-haendler-haendler) verwenden.

{% hint style="warning" %}
Komprimierte Blöcke sind noch nicht zur Nutzung als Spawner-Upgrade-Material verwendbar! Der Block wird dort ohne Betrachtung der Komprimierung als Solo-Item gewertet.
{% endhint %}

Da in der Komprimierungsliste eine Vielzahl an Items vorhanden ist, kannst du - sobald du die Komprimierung ausgewählt hast - auf ein Item in deinem Inventar klicken. Du wirst automatisch zum Komprimierungsrezept für das entsprechende Item gebracht, sofern es komprimierbar ist.\
Die Komprimierungs-Stufe lässt sich über das +/- Symbol anpassen.

### Spezial-Rezepte

GrieferGames hat auch eine Vielzahl besonderer Items, welche du herstellen kannst.

#### [Das Antike Schwert](https://items.griefergames.net/#Antikes_Schwert)

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

_Benötigte Materialien: 4 Dracheneier, 4 Leuchtfeuer, 1 Endportalrahmen_

Dieses Schwert hat eine Schärfe VIII-Verzauberung und lässt sich mit Verzauberungsbüchern in einem Amboss weiter verzaubern.

Wenn man jetzt noch eine passende Rüstung dazu hätte...?

#### [Die Cola](https://items.griefergames.net/#Cola)

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

_Benötigte Materialien: 5 Zucker, 3 Magmacreme, 1 Wassereimer_

Cola für den besonderen Kick! Dieses erfrischende Getränk gibt dir einen Schnelligkeit II-Effekt und lässt dich 90 Sekunden lang mit 40% zusätzlicher Geschwindigkeit agieren.

#### [Die Yeezys](https://items.griefergames.net/#Yeezys)

<figure><img src="../.gitbook/assets/image (4) (2).png" alt=""><figcaption></figcaption></figure>

_Benötigte Materialien: 8 Smaragde, 1 Lederschuhe_

Yeezies haben einen Geschwindigkeits- & Sprungkraft-Boost.

{% hint style="warning" %}
Durch den hohen Sprungeffekt kann man Fallschaden erleiden!\
Wir empfehlen einen NoFall-Perk bei der Nutzung.
{% endhint %}

#### Normaler Stein

_Benötigte Materialien: 8 Bruchstein, 1 Kohle_

Wer muss schon Stein im Ofen brennen, wenn man ihn auch herstellen kann?

#### [Der Dorfbewohner-Token](https://items.griefergames.net/#Dorfbewohner-Token)

<figure><img src="../.gitbook/assets/image (3) (2).png" alt=""><figcaption></figcaption></figure>

_Benötigte Materialien: 4 Smaragdblöcke, 5 Leuchtfeuer_

Wenn Dorfbewohner nicht durch den [MobRemover](server-performance.md#mobremover) entfernt werden sollen, dann kann einem dieser Token dabei helfen ihn zu schützen.

Man muss mit dem Token lediglich einen Rechtsklick auf den entsprechenden Dorfbewohner machen.&#x20;

{% hint style="info" %}
Man kann durch diese Token allerdings keine Dorfbewohner von der Farmwelt mit in die Grundstückswelt nehmen.
{% endhint %}

{% hint style="warning" %}
Der Dorfbewohner-Token schützt **nur** vor dem [MobRemover](server-performance.md#mobremover)!

Die Dorfbewohner können weiterhin normal sterben oder durch [StopLag-Maßnahmen](server-performance.md#stoplag-clearlag) gelöscht werden!
{% endhint %}

#### [Die Antike Rüstung](https://items.griefergames.net/#Antike_R%C3%BCstung_-_Komplett)

<figure><img src="../.gitbook/assets/image (1) (2) (1).png" alt=""><figcaption></figcaption></figure>

_Benötigte Materialien: insgesamt 24 Leuchtfeuer_

Jedes Rüstungsteil hat Schutz VI standardmäßig. Die perfekte Ausrüstung für einsame Farmer und gewiefte Kämpfer in der Arena. Zusammen mit dem Antiken Schwert wirst du zu einer wahren Kampfmaschine.

#### [Erschaffe Bruchstein-Generator](https://items.griefergames.net/#Erschaffe_Bruchstein-Generator)

<figure><img src="../.gitbook/assets/image (2) (2).png" alt=""><figcaption></figcaption></figure>

_Benötigte Materialien: 1 Bruchstein, 1 Eisenbarren, 1 Goldbarren, 1 Kohle, 1 Redstonestaub, 1 Lapislazuli, 1 Smaragd, 1 Diamant, 1 Lore_

Setze dieses Item in einen [passiven Spawner](../grundlagen/passive-spawner.md#passive-spawner), um ihn zu einem Bruchstein- & Erze-Generator umzufunktionieren. \
Das Item funktioniert wie ein reguläres Spawn-Ei. Ein bestehendes Spawn-Ei wird durch dieses ersetzt. Das Spawn-Ei wird nicht zurückerstattet.

#### Abschließbare Truhe

<figure><img src="../.gitbook/assets/image (154).png" alt="" width="563"><figcaption></figcaption></figure>

_Benötigte Materialien: 1 Truhe, 1 Haken, 3 Obsidian, 4 Eisenblöcke_

Platziere diese [abschließbare Truhe](../grundlagen/abschliessbare-truhen.md) auf deinem Grundstück, um sie zu verwenden. Die Truhe ist verschlossen und kann nur von dir geöffnet werden. Weitere Einstellungen kannst du über den Befehl `/chest` treffen.

### CustomBlocks

In dieser Kategorie hast du die Möglichkeit eine Vielzahl an [CustomBlocks](../grundlagen/customblocks.md) herzustellen. Diese sind vor allem zu dekorativen Zwecken gedacht und lassen dich dein Zuhause, deinen Shop oder dein Projektgrundstück noch vielseitiger dekorieren.

Auch hier kannst du einfach ein vorhandenes Item aus deinem Inventar auswählen und wirst direkt zum passenden Rezept gebracht, um weitere herzustellen.



<details>

<summary>An diesem Artikel beteiligt</summary>

* [50U7R34P3R](https://profile.griefergames.live/minecraft/8e2ce0be-aa2c-46a7-a2dc-48f948743edf)

</details>

{% hint style="danger" %}
Dieser Artikel könnte ein paar Bilder vertragen. [Interessiert](../hilfreiche-links/under-construction.md)?
{% endhint %}
