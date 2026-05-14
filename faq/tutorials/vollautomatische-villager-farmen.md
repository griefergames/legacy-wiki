---
description: und Lösungen für ale gängigen Probleme
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

# Vollautomatische Villager-Farmen

Moin 🙂&#x20;

in der Vergangenheit wurde ich häufiger mit Fragen konfrontiert, wenn es um den Bau einer effizienten und vor allem fehlerfreien Villagerfarm für Weizen, Karotten oder Kartoffeln ging. Da ich mit /p h UltraFarm auf CB21 vermutlich der Erste im Besitz einer vollkommen korrekt funktionierenden Anlage bin und sich die Anfragen in letzter Zeit gehäuft haben, möchte ich die Gelegenheit gerne nutzen, um euch alles Relevante hier zu schildern&#x20;

### Tutorial

#### 1. Aufbau & Rahmenbedingungen

<details>

<summary>1.1 Struktur und Platzierung der Farm</summary>

In 1.1 bis 1.3 wird der systematische Aufbau der Farm beschrieben. Für Funktionsweisen & Erklärungen siehe Abschnitt 2 & 3.

Die Gesamtfarm setzt sich aus der Aufeinanderstapelung beliebig vieler Teilackerflächen (im Folgenden Farmebenen genannt) zusammen, wobei auf jeder Farmebene immer nur eine Pflanze gefarmt werden soll!

Eine Farmebene umfasst dabei eine Fläche von 16x16 Ackerblöcken und muss sich zwangsläufig innerhalb eines einzigen Chunks gelegen befinden. Um diesen Chunk herum wird eine Umrandung solider Blöcke errichtet (unten dunkel-cyan) mit eingearbeiteter Eisentür, die Höhe jeder Ebene beträgt 1 Ackerschicht + 3 Luftblöcke

Für die ideale Bewässerung (blau) des Ackerbodens (braun) gilt nun folgendes Schema:&#x20;

<figure><img src="../../.gitbook/assets/image (162).png" alt=""><figcaption></figcaption></figure>

In der Praxis umgesetzt könnte eine Farmebene dann bisher etwa so aussehen (Optik natürlich variabel):

<figure><img src="../../.gitbook/assets/image (161).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary>1.2 Beleuchtung</summary>

Dieser Punkt unterscheidet je nach eurer individuellen Wahl zwischen Weizen- sowie Kartoffel-/Karottenebenen und sollte exakt wie beschrieben ausgeführt werden, da die Farm sonst unter Umständen nur eingeschränkt oder ggf. sogar überhaupt nicht funktionieren könnte.

Für Weizenebenen platziert Seelaternen (weiß) nach folgendem Schema an die Decke eurer Farmebene:

<figure><img src="../../.gitbook/assets/image (158).png" alt=""><figcaption></figcaption></figure>

Kartoffel- und Karottenebenen liegen beide folgendem Lichtschema zugrunde:

<figure><img src="../../.gitbook/assets/image (160).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary>1.3 Trichter und Lagerung</summary>

Dieser Punkt unterscheidet ebenfalls zwischen Weizen- und Kartoffel-/Karottenebenen und baut stark auf dem Trichtersystem und unendlichen Lagern auf, welche so in Vanilla-Minecraft nicht existieren und serverspezifisch sind. Gerade für neuere Spieler möchte ich daher auf folgende Wiki-Einträge verweisen:\
[Das Trichter-System](../../grundlagen/das-trichter-system.md)\
[Das unendliche Lager](../../grundlagen/das-unendliche-lager.md)\
\
Den Weizenebenen genügt das Setzen eines unendlichen Lagers mit aktiviertem Einsaugmodus an einem beliebigen Ort auf eurem GS. Optional kann auch das Auffangen von Seeds implementiert werden (ohne Sammelfunktion des unendlichen Lagers!), indem maximal ein Trichter ungefähr mittig unter jeder Weizenebene (Sammelradius: 5, Transportierte-Item-Anzahl: 64) einige Samen aufsammelt und abführt.\
\
Für Kartoffel-/Karottenebenen platziert zunächst Trichter (grau) nach folgender Anordnung unter eure jeweilige Farmebene:

<figure><img src="../../.gitbook/assets/image (164).png" alt=""><figcaption></figcaption></figure>

Nun stellt die Filter ein und setzt den Sammelradius der äußeren Trichter auf 6 und den der Inneren auf 3 Blöcke. Analog zu den Samen bei Weizen können bei Kartoffeln noch giftige Kartoffeln abgegriffen werden, geht hier wie bei den Seeds vor, nur dass ihr den Sammelradius gleich auf das Maximum einstellt. (Ein Trichter pro Ebene reicht hier wieder.)

Eine für Villager bezugsfertige Kartoffelebene könnte dann z.B. so aussehen:&#x20;

<figure><img src="../../.gitbook/assets/image (165).png" alt=""><figcaption></figcaption></figure>

</details>

#### 2. Villager

<details>

<summary>2.1  Auswahl der Villager</summary>

Für den Bau der Farm solltet ihr Farmer (keine Metzger, Fischer, etc.!) verwenden, und bestenfalls nicht auf LuckyBlock-Villager zurückgreifen oder solche, die ihr irgendwo noch herumzustehen habt, da diese womöglich bereits andere Items aufgesammelt haben könnten. Idealerweise verwendet man hierfür einen isolierten Villagerspawner und sucht sich die Farmer damit selbst zusammen. Haltet hierfür gleich ein Schwert zur Aussortierung sowie Mobtokens, ein paar Stacks eures priorisierten Anbauprodukts und einen Sammelball bereit. Ist ein Farmer gespawnt, droppt ihr ihm ein paar Stacks der Pflanze zu (zB Kartoffeln), markiert ihn mit eurem Mobtoken und verschiebt ihn über den Sammelball auf ein Feld, das am besten schon ein wenig vorbepflanzt wurde.\
\
Pro Farmebene sollten mindestens 2 Farmer, maximal jedoch 5 oder 6 untergebracht werden. Beachtet hierbei, dass der Ertrag pro Ebene mit zunehmender Villagerzahl nicht linear sondern näherungsweise beschränkt exponentiell zunimmt und somit nicht beliebig groß werden kann.

</details>

<details>

<summary>2.2 Chunks und korrektes Laden der Farm</summary>

Das Betreiben einer Villagerfarm über Chunkgrenzen hinaus provoziert mittel- bis langfristig, dass Farmer an Chunkgrenzen wegbuggen, weshalb keine Farmebene sich über diese hinweg erstrecken sollte. Auch können Villager nur getriggert werden, wenn ihr euch nicht mehr als 8 Blöcke in x-/z-Richtung von ihnen entfernt befindet - insgesamt sollte daher die gesamte Farm in einem Chunk gebaut sein und zum Laden der Anlage ein Account exakt in der Mitte dieses Chunks stehen, die Höhe y spielt hier keine Rolle.

</details>

<details>

<summary>2.3 Beheben "defekter" Villager</summary>

Unter „defekten Villagern" versteht man Farmer, welche keine / die falschen Produkte anbauen. Die Ursache hierfür lässt sich in der Prioritätenverteilung aus 3.1 finden: Entweder befinden sie sich im Endzustand 4 oder ihre Prioritätenverteilung wurde (noch) nicht getriggert. Lösungen für alle möglichen Fälle werden im Folgenden vorgestellt:\
\
Situation A: Das Tutorial in diesem Beitrag wurde größtenteils befolgt und die Villager arbeiten nicht.\
Das ist leider der Normalfall für alle neuen Farmen. Im Folgenden sind der Effektivität nach geordnet Lösungsansätze für diese Situation geschildert. Wichtig: Diese müssen simultan und regelmäßig durchgeführt werden, vermutlich mindestens eine Woche lang, um auch wirklich Ergebnisse zu erzielen:

\- Möglichst lange die Farm korrekt laden (siehe 2.2)\
\- Villager mit einem Sammelball einsammeln und neu platzieren, ggf. auch auf anderen Feldern des gleichen Anbauprodukts\
\- Neuladen des Farmchunks\
\- Serverrestarts abwarten (zuvor ggf. das GS laden)\
\- Mit Villagern handeln\
\- vollkommen andere Villager (z.B. Bibliothekare) ohne Mobtoken zeitweilig auf das Feld stellen (frisch gespawnt und möglichst ohne Items im Inventar)\
\
Situation B: Das Tutorial wurde nicht oder nicht vollständig befolgt und die Villager arbeiten nicht.\
In diesem Fall geht ihr am Besten die Punkte 1.1 bis 2.1 noch einmal gründlich durch und sucht nach konkreten Abweichungen (v.a. im Bezug auf Villager) zu eurer Farm. Besonders wichtig ist bspw., dass ihr Farmer-Villager und keine Fischer o.Ä. einsetzt, oder dass diese vorher nicht bereits irgendwo auf GrieferGames herumstanden und vielleicht andere Items eingesammelt haben. Versucht vielleicht mal, das Feld, auf dem der Villager steht, selbst anzupflanzen, oder einen zweiten / dritten Farmer dazuzugesellen. Sollte all das bei euch erfüllt bzw. nachträglich in Erfüllung gebracht (und v.a. angekaufte / Luckyblock-Villager durch neue ersetzt) worden sein, geht nach den Lösungsansätzen in Situation A vor.\
\
Situation C: Der Villager bepflanzt das Feld zwar, aber mit den falschen Anbauprodukten (z.B. mit Karotten statt Weizen).\
In diesem Fall platziert ca. 10-15 Trichter mit dem Anbauprodukt, das ihr loswerden wollt (in vorigem Beispiel wären das Karotten), als Filteritem ungefähr mittig unter die betroffene Farmebene, dreht den Sammelradius voll auf und führt die eingesammelte Abfallware ab. Nach ein paar Stunden korrekt geladener Farm könnt ihr die Trichter wieder abreißen.\
\
Situation D: Die Villager arbeiten zwar, aber nur sehr sehr langsam\
Lies dir hierfür am besten Punkt 2.2 durch & verändere ggf. den Aufbau deiner Farm\
\
Situation E: Deine Lage wird zwar durch eine der Situationen A-D beschrieben, allerdings hilft keine der Lösungsansätze weiter / Das Problem liegt ganz woanders.\
Sollten auch die Ansätze in A dir nach 2 Wochen wirklich nicht weiterhelfen, muss dein Problem wohl individuell am Schopf gepackt werden. Optional kannst du mir dann gerne eine Konvi schreiben, damit ich mir deine Farm mal genauer unter die Lupe nehmen kann.

</details>

#### 3. Funktionsweisen & Informatives

<details>

<summary>3.1 Verhaltensmuster von Farmer-Villagern</summary>

Farmer-Villager in der 1.8.9 sind von Minecraft aus ursprünglich dafür vorgesehen, Felder zu bestellen und die Erträge (Karotten, Kartoffeln und Weizen vercraftet zu Broten) an andere Villager zu verfüttern. Eine gescheite Farm zu bauen bedeutet daher nur, den Villagern die Items wegzunehmen, bevor sie diese anderweitig verwenden können. Für Weizenebenen ist das dank der unendlichen Lager ziemlich einfach, für Karotten und Kartoffeln leider nicht. Hier kommt daher Punkt 3.2 zum Einsatz, was nur dadurch möglich ist, dass alle Villageraktionen durch folgende Prioritätenverteilung bestimmt sind:

1\. Eine kleine Grundmenge an Pflanzen im Inventar haben\
2\. Freie Stellen bepflanzen\
3\. Items an andere Villager droppen\
4\. Items anhäufen

Ein Villager wird also immer erst versuchen, 1. auszuführen. Sollte das zufriedenstellend gegeben sein, geht er weiter zu 2., 3. etc. - und falls auf dem Weg dahin eine höhere Priorität nicht mehr erfüllt ist, wechselt er wieder dahin, bis er irgendwann im Endzustand 4. ankommt, was es zu vermeiden gilt.

</details>

<details>

<summary>3.2 Methode von Schattenflächen</summary>

Hierbei wird gezielt ausgenutzt, dass die Mitte eines Felds aufgrund der schlechten Beleuchtung nicht bepflanzt werden kann.

Nach der Prioritätsverteilung aus 3.1 handeln Farmer hier nämlich wie folgt: Sie sammeln in den beleuchteten Randbereichen Items und versuchen damit dann die Dunkelflächen zu bewirtschaften. Dort droppt jedoch alles und wird sofort von Trichtern aufgesammelt, bis die Villager wieder ein leeres Inventar haben und sich in den Randbereichen aufladen müssen. Bei diesem Kreisprozess werden stetig Kartoffeln / Karotten abgegriffen, ohne dass ein Inventar zu voll / zu leer wird.

</details>

<details>

<summary>3.3 "Quellen"</summary>

Dieser Punkt ist zurecht in Anführungszeichen gesetzt zu verstehen, weil die Reichweite für solche Farmen durch die Servergebundenheit natürlich zu klein ist, um irgendwo gescheite Quellen dazu zu finden. Alle hier angegebenen Informationen wurden demnach von mir persönlich über die letzten 2-3 Jahre hinweg empirisch gesammelt und sind nicht unfehlbar, wenn auch zu sehr zufriedenstellenden Quoten reproduzierbar. Trotzdem bin ich immer offen für alternative Lösungsansätze und Ideen&#x20;

</details>



<details>

<summary>An diesem Artikel beteiligt</summary>

* [UltraLuca](https://profile.griefergames.net/minecraft/603ddc86-2f72-4763-83bf-3c33cca9ab55)
* [50U7R34P3R](https://profile.griefergames.net/minecraft/8e2ce0be-aa2c-46a7-a2dc-48f948743edf)

</details>
