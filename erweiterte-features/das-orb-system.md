---
description: Aufbau und Übersicht der Orb-NPC und des Orb-Systems
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
---

# 🔘 Das Orb-System

Auf dem 1.8-Netzwerk wurde 2020 eine neue [Währung](../grundlagen/waehrungen.md) und ein dazu passendes System vorgestellt: Das Orb-System. Ganz kurz und knapp gesagt ist das Orb-System eine neue Möglichkeit für Spieler, durch das Farmen an wertvolle Items zu kommen.

Du kannst auf jedem der 25 Citybuild-Server mit den Befehlen `/warp Orbs` und `/warp Stadt` zu den [Orb-NPC](die-hauptstadt.md#orb-haendler-orb-verkaeufer-und-statistik) zu kommen. Hier siehst du nun 3 verschiedene NPC, die zu dem System gehören.

### Der Orb-Händler "Händler"

<figure><img src="https://lh5.googleusercontent.com/krOnlUNEx6xk8qdN5kUWmmImPeXsbNHUhOjZdqUUdgNMKD9jKHoryIc1Om8YuG4PoHrmSpRGkQE2V2nYXbz6Q8wNJn-XeAzu_srA_PiOtef1XokmfrJDwveqCRKc79XDOfnpfSgABDU4WcuB3AnnfIM" alt=""><figcaption><p>Der Orb-Händler an seinem Stand</p></figcaption></figure>

Beim Händler könnt ihr eure erfarmten Items eintauschen, um im Gegensatz [Orbs](../grundlagen/waehrungen.md#orbs) zu erhalten. Hierfür sind nahezu alle Items im Menü des Händlers vorhanden.

Hier könnt ihr dann in den Unterkategorien euer Item finden. Wenn ihr zum Beispiel Stein gefarmt habt, findet ihr die Abgabe für Stein in der "Steine"-Kategorie. Dort klickt ihr dann auf Stein. Nun könnt ihr eure Items abgeben.&#x20;

{% hint style="success" %}
Wenn ihr im Menü des Orb-Händler seid und ein Item in eurem Inventar anklickt, gelangt ihr direkt zum Eintausch, sofern der Orb-Händler das Item entgegen nimmt.
{% endhint %}

Zur Auswahl stehen die Abgabe einzelner Items, einem Stack des Items oder aller Items dieser Art aus eurem Inventar (per Klick auf den Trichter).

<figure><img src="https://lh4.googleusercontent.com/4gG_AmkonwnnBQYKBTZu4xegRYsZiz0tgNxt7f5XnFRHGvzFCj9LBpgMxkPE6qod0mfTxGYeycS42KWRRsT2o78lH-Tc5bK8_73Q9esdhUEkUI9A-Uivj4NpDYYOF55_YYxV1ToGpq2vg0-3MzHJBYU" alt=""><figcaption><p>Der Orb-Händler kauft eure Items an</p></figcaption></figure>

{% hint style="warning" %}
Besondere Items (bspw. Admin-Items oder abweichende Namen/Signatur/NBT) werden vom System nicht gesondert erkannt/behandelt!
{% endhint %}

Je seltener und schwerer das Item zu farmen ist, desto mehr Orbs gibt es für das Item.

Der Preis jedes Items täglich um 18 Uhr zurückgesetzt. Das heißt, zu bestimmten Uhrzeiten bekommt ihr teilweise mehr Orbs für eure Items. Je mehr Items nun von einem Item-Typ auf dem Citybuild-Server abgegeben werden, desto weniger Orbs bekommst du bei der nächsten Abgabe der Items. Dafür gibt es zwei Preisfall-Stufen.

Wenn eine bestimmte Anzahl an abgegebenen Items erreicht wird, greift der Preisfall und jeder Spieler auf dem Citybuild-Server bekommt weniger Orbs für diese Item-Art. Der resultierende Preis verbleibt bis zum nächsten Preisreset für jeden Spieler.

<details>

<summary>Beispiel Steine</summary>

1. Preis: 1 Stein = 20 Orbs
2. Preis: 1 Stein = 15 Orbs
3. Preis: 1 Stein = 10 Orbs

</details>

{% hint style="danger" %}
Enige Items haben zudem eine Preisfallstufe, welche die Menge auf unter 1 Orb setzt.\
Kakteen erzielen bspw. im zweiten Preisfall nur 0,2 Orbs.

Die Anzeige "0 Orbs" ist hier ein bekannter Fehler, welchen wir leider nicht beheben können. Die Orbs werden dennoch korrekt berechnet und ausgegeben.
{% endhint %}

Der Orb-Händler erkennt auch komprimierte Items und gibt euch passend Orbs für die komprimierte Item-Anzahl im Austausch.

{% hint style="warning" %}
Ihr könnt maximal 4.782.969 Items auf einmal abgeben. Das entspricht einem maximal komprimierten Stufe-7-Block.
{% endhint %}

### Der Orb-Verkäufer "Verkäufer"

<figure><img src="https://lh5.googleusercontent.com/XfZEjljpjgWB0KxLhPsAXiRS8M0uUHWJSxOCXZc8ASr5Ioquu13enLn0yAo9WTJwLaVYV66Td4KvNNtZ6AS9p5f_YxZIGlEqGKdEfUjhP10TsnBqoT5QwQfCrJtWcKV4CdjNgQRcZsfmPBPCjaWuiqA" alt=""><figcaption><p>Der Orb-Verkäufer an seinem Stand</p></figcaption></figure>

Ihr habt nun also einige Orbs durch Farmen erhalten. Was macht ihr jetzt damit?&#x20;

Beim Orb-Verkäufer könnt ihr wie in einem Shop verschiedene Items mit euren Orbs kaufen.&#x20;

Öffnet das Menü des Verkäufers und euch werden verschiedene Kategorien angeboten. In diesem Menü könnt ihr über den "Geldsack-Kopf" eure aktuell gesammelten Orbs sehen.

{% tabs %}
{% tab title="Perks" %}
In dieser Kategorie könnt ihr euch drei verschiedene Perks kaufen, welche normalerweise nur durch GrieferGames-$ oder durch Kisten erhaltbar sind.
{% endtab %}

{% tab title="Partikel" %}
In dieser Kategorie könnt ihr euch drei verschiedene Partikel kaufen, welche nur hier erhältlich sind.
{% endtab %}

{% tab title="Spezielle Items" %}
In dieser Kategorie könnt ihr euch spezielle Items kaufen.&#x20;

Hier gibt es “Trophäen” wie den [Kaktus-](https://items.griefergames.net/#Orb-Items_%7C_Kaktusk%C3%B6nig) und [Kürbiskönig](https://items.griefergames.net/#Orb-Items_%7C_K%C3%BCrbisk%C3%B6nig).

Ebenso finden sich hier nützliche Dinge, wie Upgrades für passive Spawner, Flug-/Abbautränke und magische Items, mit welchen ihr zum Beispiel mit einem Eimer 1000 Wasserblöcke setzen könnt.
{% endtab %}

{% tab title="Orb-Rüstung" %}
In dieser Kategorie gibt es eine Rüstung, die besser ist als alles, was du selber herstellen kannst. Damit bist du ein wahrer Krieger und sehr gut auf deinen Reisen geschützt.
{% endtab %}

{% tab title="Farming-Items" %}
In dieser Kategorie gibt es spezielle Werkzeuge, mit denen ihr zum Beispiel einen ganzen Baum oder ein 3x3 Feld an Blöcken auf einmal abbauen könnt.
{% endtab %}
{% endtabs %}

### Die Orb-Statistik "Statistik"

<figure><img src="https://lh3.googleusercontent.com/un9Z2LyE9vCxvixmYl_isYaRP48uCfRBsHOKWmc8_tPGnDcr77LUWLbX48bSKUQd0LD6K_7LGcKVT6BJLuXMBjRX8KFkNLDutXPMi5IyX7h87X4sILS_XYlGsPZulKtx1aUhQGp9tO4B0CS32CqBYPU" alt=""><figcaption><p>Der Statistik-NPC an seinem Stand</p></figcaption></figure>

Der letzte NPC des Orb-Systems ist der Statistik-NPC.

Über diesen findet ihr ein Menü mit allen Items im Orb-System und eine Rangliste, welche die Spieler auflistet, welche die meisten Items einer Art abgegeben haben.\
Hierüber könnt ihr euren Fortschritt mit dem anderer Spielern vergleichen und darauf hin arbeiten der Spieler zu sein, der die meisten Items einer Art abgegeben hat.

### Die Zukunft des Orb-System

{% hint style="info" %}
Seit einiger Zeit wird das Orb-System immer häufiger kritisiert und ein Update wird gefordert. Das Team hat hierzu mitgeteilt, dass das Orb-System dafür komplett überarbeitet werden muss. Ein Update wird also noch etwas brauchen.
{% endhint %}



<details>

<summary>An diesem Artikel beteiligt</summary>

* [BentosMentos](https://profile.griefergames.live/minecraft/813d7454-3f9f-449d-9010-b3ee225e56aa)
* [50U7R34P3R](https://profile.griefergames.live/minecraft/8e2ce0be-aa2c-46a7-a2dc-48f948743edf)

</details>
