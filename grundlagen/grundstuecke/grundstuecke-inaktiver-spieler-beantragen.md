---
description: Funktion und Ablauf des Checkplot-System
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

# Grundstücke inaktiver Spieler beantragen

GrieferGames ist nun schon seit 2016 als Citybuild Server für die Spieler da. Da kommt es natürlich vor, dass einige Spieler den Server nach einiger Zeit wieder verlassen.

Du möchtest nun aber an einem Bauprojekt weiter bauen, aber alle Grundstücke um deines sind schon im Besitz von anderen Spielern?\
Mit dem Checkplot-System kannst du diese beantragen.

### Ablauf eines Antrag im Checkplot-System

Um ein Grundstück neben deinem zu Checkploten, musst du auf das Grundstück gehen und den Befehl `/checkplot` eingeben. Nun erhältst du eine Nachricht in den Chat.

{% hint style="info" %}
&#x20;Du kannst nur inaktive Grundstück in der Nähe eines deiner Grundstücke beantragen.\
\
**Spawn-GS Besonderheiten:** Um den Spawn herum gibt es Spawn-Grundstücke, die von Spielern mit hohem Wert gehandelt werden. Diese Grundstücke befinden sich in der 1. bis 5. Grundstücksreihe direkt um den Spawn herum und können **nicht** über `/checkplot` beantragt werden. Sollte ein Spawn-Grundstück inaktiv oder unbebaut sein, kann es über `/spawnplotreport` gemeldet werden.&#x20;
{% endhint %}

Lässt sich das Grundstück nicht betreten, weil das durch den Besitzer verboten wurde, kannst du den Antrag durchführen, indem du vor dem Grundstück stehst und den [Befehl](../befehlsuebersicht/spezielle-features/checkplot.md) eingibst, während du auf das Grundstück schaust.

<details>

<summary>Befehl mit ID</summary>

Alternativ kannst du das Grundstück auch über die Grundstücks-ID beantragen.

* /checkplot \[Grundstücks-ID]
* /checkplot antrag \[Grundstücks-ID]
* /checkplot claim \[Grundstücks-ID]
* /checkplot claim confirm \[Grundstücks-ID]

</details>

<figure><img src="https://lh5.googleusercontent.com/B8ReErIT6ftnDkFpl_v89XHQuveXLUixrZq54x8jGMCttvbSqOwuXwlQ2-h-dhFV8OSoyhZBL06dMQt8zOS0HKBPqsuiDGwq4X3FO-H3U-fSOY2vL_InMeTx_62BjE2xh-OCh_D_pwAHaxo_Rcay2SU" alt=""><figcaption><p>Rückmeldung im Chat nach Eingabe von <code>/checkplot</code></p></figcaption></figure>

In dieser Nachricht stehen nun weitere Informationen. Zum einen steht oben, wann der Grundstücksbesitzer das letzte Mal online war. Ein Spieler muss einen gewissen Zeitraum offline gewesen sein, damit du das Grundstück beanspruchen kannst.

In der Nachricht stehen nun zwei weitere Daten. Das erste Datum zeigt dir, wann du ein unbebautes Grundstück beantragen kannst. Das zweite Datum zeigt dir, wann du das Grundstück beantragen kannst, wenn es baulich verändert wurde.

Wenn das aktuelle Datum nach den Daten des Systems ist, kannst du deinen Antrag mit `/checkplot antrag` einreichen.

Baulich unveränderte Grundstücke werden vom System automatisch freigegeben.&#x20;

Wenn das Grundstück bebaut ist, wird der Antrag von einem Teammitglied geprüft und du bekommst zeitnah eine Nachricht, ob du das Grundstück übernehmen kannst.

{% hint style="info" %}
Den Status deiner Anträge kannst du jederzeit mit `/checkplot list` einsehen.
{% endhint %}

Wenn ein Grundstück freigegeben wurde, kannst du es mit `/checkplot claim` beanspruchen und darauf folgend mit `/checkplot claim confirm` die Übernahme bestätigen.

{% hint style="warning" %}
Ein Grundstück kannst du nur annehmen, wenn du noch ein weiteres Grundstück auf dem CB besitzen kannst. Solltest du keinen freien Grundstücks-Slot haben, musst du 10.000$ für den Kauf eines weiteren Grundstücks zahlen.
{% endhint %}

{% hint style="success" %}
Wenn du Fragen zu deinem Antrag hast, kannst du diese auch direkt dem Teamler stellen, der die Checkplot-Anträge auf deinem Citybuild-Server prüft.

Die [Liste der zuständigen Teammitgliede](../../faq/griefergames/team.md)r findest du in den FAQ.
{% endhint %}

#### Ablehnungsgründe

Wenn dein Antrag abgelehnt wird, so kann dies unterschiedliche Gründe haben.

{% tabs %}
{% tab title="Antrag lässt sich nicht erstellen" %}
* Der Besitzer des Grundstück ist noch nicht lange genug offline.
* Du besitzt kein eigenes Grundstück im Umkreis von 2 Grundstücken.
* Du hast bereits 5 offene Anträge im System, welche geprüft werden müssen.
* Das Grundstück ist ein Merge-Grundstück.
* Das Grundstück befindet sich in den ersten 5 Reihen um das Spawn-Grundstück des Citybuild-Servers.
* Das Grundstück wurde bereits von einem anderen Spieler beantragt.
* Das Grundstück gehört einem Spieler, welcher einen besonderen Rang hat. (Teammitglieder, Freunde, Content-Creator, etc.)
* Dein Antrag auf das Grundstück wurde in den letzten 14 Tagen durch ein Teammitglied abgelehnt.
{% endtab %}

{% tab title="Antrag von Teammitglied abgelehnt" %}
* Deine Grundstücke in der Nähe sind nicht ausreichend bebaut.
* Das beantragte Grundstück ist wertvoll bebaut oder hat wertvolle Items in Truhen.
* Das beantragte Grundstück trägt einen wertvollen Alias.
{% endtab %}
{% endtabs %}

#### Ein Merge beantragen

Mit dem Checkplot-System kannst du keine Merge-Grundstücke beantragen. Dafür gibt es aber eine andere Lösung. Du kannst eine [Grundstücks-Verschiebung](grundstucke-verschieben-and-erweitern.md) beantragen.

Wenn du diesen Weg der Grundstücksverschiebung wählst kann es vorkommen, dass dein Grundstück verschoben wird. In der Regel wird immer das Grundstück verschoben, bei welchem dies sinnvoller ist.

{% hint style="warning" %}
Dies ist ein freiwilliger Service seitens des Teams, weshalb eine Verschiebung nicht immer erfolgen muss und manchmal auch mehrere Tage bis Wochen dauern kann.
{% endhint %}



<details>

<summary>An diesem Artikel beteiligt</summary>

* [BentosMentos](https://profile.griefergames.live/minecraft/813d7454-3f9f-449d-9010-b3ee225e56aa)
* [50U7R34P3R](https://profile.griefergames.live/minecraft/8e2ce0be-aa2c-46a7-a2dc-48f948743edf)

</details>
