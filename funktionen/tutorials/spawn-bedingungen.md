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
    visible: false
  tags:
    visible: true
---

# Tutorial für Spawn-Bedingungen

Moin Leute,\
GrandMagus22 und ich haben uns mal zusammengesetzt, um für euch ein kleines Tutorial zu erstellen, was Mobs und deren Spawn-Voraussetzungen angeht. Das Ganze wollen wir euch hier tabellarisch aufzählen, damit ihr direkt erkennen könnt, wo ein Fehler liegt, sollte ein Spawner mal nicht funktionieren.

„N/A“ bedeutet in der Tabelle, dass es für diesen Punkt keine besondere Voraussetzung gibt.

<table data-header-hidden><thead><tr><th width="153"></th><th></th><th></th><th></th><th></th></tr></thead><tbody><tr><td><strong>Mobs</strong></td><td><strong>Höhe (y-Achse)</strong></td><td><strong>Lichtlevel</strong></td><td><strong>Biome</strong></td><td><strong>Besonderheiten</strong></td></tr><tr><td>Creeper</td><td>N/A</td><td>&#x3C; 7</td><td>N/A</td><td>N/A</td></tr><tr><td>Dorfbewohner</td><td>N/A</td><td>N/A</td><td>N/A</td><td>N/A</td></tr><tr><td>Enderman</td><td>N/A</td><td>&#x3C; 7</td><td>N/A</td><td>3 Blöcke nach oben frei</td></tr><tr><td>Endermilbe</td><td>N/A</td><td>N/A</td><td>N/A</td><td>N/A</td></tr><tr><td>Fledermaus</td><td>&#x3C; 63</td><td>&#x3C; 3</td><td>N/A</td><td>N/A</td></tr><tr><td>Ghast</td><td>N/A</td><td>N/A</td><td>N/A</td><td>Großes Spawngebiet erforderlich – dürfen das Grundstück NICHT verlassen</td></tr><tr><td>Kaninchen</td><td>N/A</td><td>N/A</td><td>N/A</td><td>N/A</td></tr><tr><td>Hexe</td><td>N/A</td><td>&#x3C; 7</td><td>N/A</td><td>N/A</td></tr><tr><td>Höhlenspinne</td><td>N/A</td><td>N/A</td><td>N/A</td><td>N/A</td></tr><tr><td>Huhn</td><td>N/A</td><td>> 9</td><td>N/A</td><td>Grasblöcke als Boden</td></tr><tr><td>Kuh</td><td>N/A</td><td>> 9</td><td>N/A</td><td>Grasblöcke als Boden</td></tr><tr><td>Lohe</td><td>N/A</td><td>&#x3C; 11</td><td>N/A</td><td>N/A</td></tr><tr><td>Magmaschleim</td><td>N/A</td><td>N/A</td><td>N/A</td><td>Spawner nicht direkt nebeneinander platzieren</td></tr><tr><td>Ozelot</td><td>63</td><td>N/A</td><td>JUNGLE</td><td>Grasblöcke als Boden</td></tr><tr><td>Pferd</td><td>N/A</td><td>N/A</td><td>PLAINS, SAVANNA, SWAMPLAND</td><td>N/A</td></tr><tr><td>Pilzkuh</td><td>N/A</td><td>> 9</td><td>N/A</td><td>Myzel als Boden</td></tr><tr><td>Schaf</td><td>N/A</td><td>> 9</td><td>N/A</td><td>Grasblöcke als Boden</td></tr><tr><td>Schwein</td><td>N/A</td><td>> 9</td><td>N/A</td><td>Grasblöcke als Boden</td></tr><tr><td>Silberfisch</td><td>N/A</td><td>&#x3C; 11</td><td>N/A</td><td>N/A</td></tr><tr><td>Skelett</td><td>N/A</td><td>&#x3C; 7</td><td>N/A</td><td>N/A</td></tr><tr><td>Schleim</td><td>51 - 69</td><td>&#x3C; 7</td><td>SWAMP</td><td>Spawner nicht direkt nebeneinander platzieren</td></tr><tr><td>Spinne</td><td>N/A</td><td>&#x3C; 7</td><td>N/A</td><td>N/A</td></tr><tr><td>Tintenfisch</td><td>47 - 63</td><td>N/A</td><td>N/A</td><td>N/A</td></tr><tr><td>Wächter</td><td>N/A</td><td>N/A</td><td>N/A</td><td>N/A</td></tr><tr><td>Wolf</td><td>N/A</td><td>N/A</td><td>N/A</td><td>Spawnt nur auf Gras</td></tr><tr><td>Schweinezombie</td><td>N/A</td><td>&#x3C; 7</td><td>N/A</td><td>N/A</td></tr><tr><td>Zombie</td><td>N/A</td><td>&#x3C; 7</td><td>N/A</td><td>Auf allen ganzen Blöcken, außer transparenten</td></tr></tbody></table>

Wir beide sind keine Experten, also kann es sein, dass sich der eine oder andere Fehler eingeschlichen hat – gerade was Spawn-Bedingungen für natürliche Spawns oder für Spawner angeht. Wenn wir etwas aus eigener Erfahrung ausschließen konnten, haben wir das auch gemacht. Bei Zweifeln haben wir es lieber drin gelassen – wir lassen uns gerne korrigieren.

Natürlich kann es auch sein, dass in der Tabelle manche Dinge fehlen. Habt ihr was? Immer her damit!

Ich hoffe, dass euch dieses Tutorial über Spawn-Bedingungen hilft!\
Beste Grüße\
GrandMagus22 und 1Waschbaer

{% hint style="warning" %}
Achtung! Es gibt keine Garantie für die Richtigkeit/Vollständigkeit der Angaben! Wir haften für keine Verluste.
{% endhint %}

<details>

<summary>An diesem Artikel beteiligt</summary>

* [GrandMagus22](https://profile.griefergames.net/minecraft/94b5fbe3-0ffa-43bf-a2e6-377581a17e5c)
* [1Waschbaer](https://profile.griefergames.net/minecraft/fc3a2003-5bd3-49a7-b1db-d2867b6a0f01)
* [50U7R34P3R](https://profile.griefergames.net/minecraft/8e2ce0be-aa2c-46a7-a2dc-48f948743edf)

</details>
