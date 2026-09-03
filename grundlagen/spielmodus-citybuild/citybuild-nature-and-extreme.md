---
description: Besonderheiten von Citybuild Nature & Extreme
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

# 🏔️ Citybuild Nature & Extreme

Die Citybuild-Server erreicht man über den Portalraum, über das Auswahlmenü unter dem Befehl `/switch`  oder direkt mit dem Befehl `/switch nature` für Citybuild Nature oder `/switch extreme` für Citybuild Extreme.

<figure><img src="../../.gitbook/assets/image (73).png" alt=""><figcaption></figcaption></figure>

Die Plotwelt dieser Citybuild-Server ist nicht standardisiert und besteht aus einer normalen Minecraft-Welt, welche in einzelne [Grundstücke](../grundstuecke/) aufgeteilt ist.

* Jedes Grundstück ist 42x42 Blöcke groß.
* Grundstücke haben keinen [Rand](../grundstuecke/grundstuecke-veraendern.md#rand) und grenzen direkt aneinander.
* Zwischen den Grundstücken ist **keine** Straße.
* Das Grundstück wird automatisch mit der normalen Weltgenerierung auf Basis des Bioms erzeugt. Die Höhe und Art der Blöcke ist also völlig unterschiedlich.
* Die maximale Bauhöhe liegt bei 256.

<figure><img src="../../.gitbook/assets/image (7) (1) (1).png" alt=""><figcaption></figcaption></figure>

Nebeneinander liegende Grundstücke, die du besitzt, kannst du zu einem großen [Grundstück verbinden](../grundstuecke/grundstuecke-verbinden.md). Auf Citybuild Nature & Extreme ist dies aber lediglich für Wasser-/Lava-Fluss über die Grundstücksgrenze sowie die Komfort-Funktionen des [Trichter-Systems](../das-trichter-system.md) erforderlich. In den meisten Fällen verzichten Spieler auf das Verbinden der Grundstücke auf diesem Server.

{% hint style="danger" %}
Wird ein Grundstück auf den Citybuild-Servern Nature/Extreme zu häufig zurückgesetzt, kommt es zu einem Fehler, bei welchem keine Blöcke mehr auf dem Grundstück droppen.

Dies gilt sowohl für natürlich generierte Blöcke beim Abbau, als auch für Items, die ein Spieler abwirft/verliert.

Der Fehler behebt sich zum nächsten Server-Neustart selbstständig. Verlorene Items können nicht erstattet werden.
{% endhint %}



### Besonderheiten

* Plotwelt mit natürlicher Weltgenerierung
* größere Grundstücke
* kein Rand, keine Straßen
* erhöhter Cooldown beim Zurücksetzen/Löschen von Grundstücken
* Angepasster [MobRemover](../../erweiterte-features/server-performance.md) (chunkbasiert)
