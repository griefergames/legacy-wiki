---
description: Befehle zum Verwalten von Hologrammen (/pholo)
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

# Hologramme

Mit diesen Befehlen kannst du Hologramme auf deinen Grundstücken verwalten. Welche Ränge Hologramme verwalten können, findest du unter [Rang-Rechte](../rang-befehle.md). Weitere Infos findest du unter [Spawner, Hologramme & Partikeleffekte verwalten](../../grundstuecke/spawner-hologramme-and-partikeleffekte-verwalten.md).

| Befehl | Funktion |
| --- | --- |
| `/pholo` | Listet alle Hologramm-Befehle auf |
| `/pholo help` | Zeigt alle verfügbaren Befehle an |
| `/pholo list` | Zeigt alle Hologramme, die du auf diesem Citybuild-Server hast |
| `/pholo create <Nummer> <Text>` | Erzeugt an deiner Position ein Hologramm mit dieser Nummer |
| `/pholo remove <Nummer>` | Löscht das Hologramm mit dieser Nummer |
| `/pholo add` | Fügt eine neue Zeile zum Hologramm hinzu |
| `/pholo edit <Nummer> <Zeilennummer> <Text>` | Ändert die angegebene Zeile des Hologramms |
| `/pholo move <Nummer>` | Verschiebt das Hologramm auf deine aktuelle Position |
| `/pholo tp <Nummer>` | Teleportiere dich zum Hologramm mit dieser Nummer |
| `/pholo removeplot` | Entfernt alle Hologramme auf dem Grundstück |

## [#](#hinweise)Hinweise

Hologramme erstellst und verschiebst du nur auf deinem eigenen Grundstück.Ein Hologramm hat höchstens **3 Zeilen**.Mit `&` und einem Farbcode färbst du den Text ein, z. B. `&6` für Gold.Umlaute sind erlaubt, andere Sonderzeichen nicht.

{% hint style="info" %}
Schreibst du `{displayname}` in eine Zeile, sieht jeder Besucher an dieser Stelle seinen eigenen Namen. So kannst du z. B. jeden Gast persönlich begrüßen.
{% endhint %}
