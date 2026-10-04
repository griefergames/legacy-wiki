---
description: Funktion und Ablauf von /setowner
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

# Grundstücke überschreiben

Du kannst natürlich auch mit Grundstücken handeln oder diese an andere Spieler verschenken. Dafür kannst du Grundstücke an andere Spieler überschreiben.

Je nach Größe des Grundstücks läuft das etwas unterschiedlich ab:

## Normale Grundstücke überschreiben

Einzel-Grundstücke können jederzeit mit `/setowner <NAME>` zur Übertragung an einen anderen Spieler reserviert werden. 
Damit die Überschreibung durchgeführt wird, müssen sowohl der bisherige als auch der neue Besitzer diese mit `/setowner confirm` bestätigen. Zum ablehnen der Übertragung kann der Befehl `/setowner deny` verwendet werden. 
Für jede Bestätigung stehen **30 Sekunden** zur Verfügung. Erfolgt innerhalb dieser Zeit keine Bestätigung, läuft die Anfrage ab.

{% hint style="warning" %}
Hat der neue Besitzer keine freien Grundstücke auf dem jeweiligen Citybuild-Server, fallen für die Übertragung eines Einzel-Grundstücks **10.000 $** an.
{% endhint %}

## Große Grundstücke überschreiben

Merge-Grundstücke bis zu einer Größe von 25 Grundstücken gelten als große Grundstücke.

Der Ablauf bei der Überschreibung ist der gleiche wie bei normalen Grundstücken. Die Übertragung von Merge-Grundstücken ist generell kostenlos.

## Riesige Grundstücke überschreiben

Ab einem 26er-Merge zählt ein Grundstück als riesiges Grundstück. Der Ablauf bei der Überschreibung ist der gleiche wie bei normalen Grundstücken.

Diese Grundstücke kannst du – im Gegensatz zu normalen und großen Grundstücken – nur alle 7 Tage überschreiben. Den Cooldown dafür kannst du über `/cooldowns` einsehen.
