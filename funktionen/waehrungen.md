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
  anchors:
    visible: true
---

# 💰 Währungen

In eurer **Brieftasche** seht ihr euer Bargeld, euer Bankguthaben, eure Kristalle, Adventurer-Coins, Swap-Tokens und Prestige-Tokens auf einen Blick. Statt `/wallet` oder `/brieftasche` funktioniert auch `/portemonnaie`.

## GrieferGames-Dollar

GrieferGames-Dollar ($) werden als allgemein gültiges Zahlungsmittel auf unserem 1.8-Netzwerk verwendet, um den Handel zwischen Spielern zu vereinfachen. Ihr könnt Geld verdienen, indem ihr direkt mit Spielern untereinander [Items handelt](features/der-handel.md) oder [Jobs](features/das-job-system.md) (`/jobs`) erfüllt. Geld wird auch zum Bezahlen von verschiedenen Serverfunktionen eingesetzt.

$ werden auf verschiedenen Wegen in das Spielgeschehen eingebracht.

Spieler können ihre $ entweder mit sich führen (Kontostand) oder auf der Bank sichern (Bankguthaben). Geld auf der Bank steht nicht für die Verwendung zur Verfügung, bis es vom Spieler abgehoben wird. Ein- und Auszahlungen sind ab **1.000 Dollar** möglich.

Beim Bezahlen von Serverfunktionen wird das Geld automatisch vom Kontostand abgezogen. Zum Überweisen an Spieler oder zum Übertragen zwischen Bankguthaben und Kontostand werden [Befehle](befehlsuebersicht/allgemeine-befehle.md#allgemeine-befehle) verwendet.

#### Moneylog

Viele Transaktionen kannst du über den Befehl `/moneylog` anzeigen lassen. Neben Zahlungen zwischen Spielern und Buchungen der Bank findest du dort auch Geld aus dem CaseOpening, dem Block des Tages, den Jobs, dem Auktionshaus, der Lotterie, den Advancements und den Fragmenten.

Standardmäßig zeigt der Moneylog die letzten **30 Tage**. Über den **Filter** kannst du:

* einzelne Bereiche ein- und ausblenden,
* den Zeitraum zwischen 24 Stunden und 30 Tagen wählen,
* nach einem bestimmten Datum suchen.

Mit der **Spielersuche** siehst du nur die Einträge mit einem bestimmten Spieler. Eine Statistik fasst deine Einnahmen und Ausgaben im gewählten Zeitraum zusammen.

## Kristalle

Kristalle sind eine Premium-Währung, welche zum Kauf von Kisten am [Case-Opening](features/das-case-opening.md) eingesetzt werden kann.

Kristalle können über den [In-Game-Store](features/das-case-opening.md#in-game-store) oder den [GrieferGames WebShop](https://store.griefergames.net) erworben oder durch Spielaktivitäten erspielt werden. Klickst du z. B. ein Teammitglied oder einen Spieler mit Hero-Rang an, bekommst du **einmalig** einen zufälligen Betrag an Kristallen.

Sie sind **nicht handelbar** und können daher nicht als Zahlungsmittel zwischen 2 Spielern genutzt werden.

Deinen aktuellen Kristall-Kontostand zeigt dir der Befehl `/kristalle`. Das Gutschreiben und Einsetzen deiner Kristalle in den letzten **30 Tagen** kannst du über den Befehl `/kristalllog` prüfen.

## Prestige-Tokens

Durch Käufe von **Kristallen oder Kisten mit Echtgeld im In-Game-Store** erhaltet ihr **Prestige-Tokens**. Diese könnt ihr im Prestige-Shop für besondere Vorteile und Angebote einlösen. Den Prestige-Shop findet ihr am Spawn.

<figure><img src="../.gitbook/assets/9azNxrf.png" alt="Prestige-Shop" width="456"><figcaption></figcaption></figure>

Weitere Informationen dazu gibt es im Beitrag „[Das Case-Opening](features/das-case-opening.md)“.

Prestige-Tokens sind **nicht handelbar** und können daher nicht als Zahlungsmittel zwischen 2 Spielern genutzt werden.

## Orbs

[Orbs](features/das-orb-system.md) sind eine Serverwährung, welche beim [Orb-Händler](features/das-orb-system.md#der-orb-haendler-haendler) erhältlich ist. Orbs werden im Tausch gegen Items generiert, welche der Server entgegennimmt. Spieler können daher unbegrenzt Orbs durch Spielaktivität selbst erzeugen.

<figure><img src="../.gitbook/assets/5NHEiLg.png" alt="Orb-Händler und Orb-Verkäufer" width="563"><figcaption></figcaption></figure>

Orbs können beim [Orb-Verkäufer](features/das-orb-system.md#der-orb-verkaeufer-verkaeufer) eingesetzt werden, um spezielle Items und optische Features zu erwerben. Sie sind **nicht handelbar** und können daher nicht als Zahlungsmittel zwischen 2 Spielern genutzt werden.

## Adventurer-Coins

Adventurer-Coins (oder kurz „Coins“) sind eine Serverwährung, welche beim [Adventurer](features/das-adventurer-system.md#adventurer) erhältlich ist. Coins werden durch das Erledigen von Aufgaben für den Adventurer generiert. Spieler können daher nur zeitlich begrenzt eine bestimmte Menge an Coins durch Spielaktivität generieren.

<figure><img src="../.gitbook/assets/Xyh25sq.png" alt="Adventurer und Admin-Shop" width="563"><figcaption></figcaption></figure>

Coins können beim [Admin-Shop](features/das-adventurer-system.md#der-admin-shop) eingesetzt werden, um spezielle Items sowie optische und funktionelle Features zu erwerben. Adventurer-Coins sind **nicht handelbar** und können daher nicht als Zahlungsmittel zwischen 2 Spielern genutzt werden.

## Swap-Token

Swap-Tokens sind eine saisonale Währung, welche vor allem zu besonderen Anlässen temporär im Spiel nutzbar ist. Tokens kann man durch die Abgabe von Items bei einem Tausch-NPC erhalten. Hierbei bekommt man verschieden viele Tokens für verschiedene Items.

<figure><img src="../.gitbook/assets/kPe4B6e.png" alt="Tausch-NPC (hier der Tausch-Taucher)"><figcaption></figcaption></figure>

{% hint style="info" %}
In der Vergangenheit gab es zur Weihnachtszeit 2024 die Tausch-Elfe, zu Ostern 2025 den Tausch-Hasen oder auch im Sommer 2026 den Tausch-Taucher.
{% endhint %}

Für gängige Admin-Items wie [Grundgestein](https://items.griefergames.net/#Grundgestein), [Barrieren](https://items.griefergames.net/#Barriere) oder [Dracheneier](https://items.griefergames.net/#Drachenei) kann man einen Swap-Token gutgeschrieben bekommen. Für spezielle saisonale Items, welche man aus dem CaseOpening ziehen kann, erhält man bis zu 5 Swap-Tokens.

Von den Swap-Tokens kann man sich beim selben NPC dann im Token-Shop Kisten für das Case-Opening, bekannte begehrte Items oder sogar exklusive Items und Item-Variationen kaufen.

Swap-Tokens sind **nicht handelbar** und können daher nicht als Zahlungsmittel zwischen 2 Spielern genutzt werden.

{% hint style="warning" %}
Bitte beachte, dass die Swap-Tokens immer nur für den derzeitigen Token-Shop nutzbar sind, sie verfallen also, wenn der temporäre NPC wieder weg ist.
{% endhint %}
