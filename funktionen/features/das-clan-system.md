---
description: Warum alleine losziehen, wenn es viel mehr Spaß macht, gemeinsam zu spielen?
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

# 👥 Clan-System

Das überarbeitete Clan-System gibt es seit dem 09.07.2019. Es ist der Nachfolger des alten Clan-Plugins von 2018, welches aufgrund von kritischen Fehlern eingestellt wurde.

In einem Clan kann man sich mit anderen Spielern zusammentun, um gemeinsam zu spielen, sich gegenseitig zu unterstützen und gemeinsame Ziele zu erreichen.

Ein Clan besteht aus einem Clan-Leiter und seinen Clan-Mitgliedern. Jedes Mitglied hat eine [Rolle](das-clan-system.md#clan-rollen), die festlegt, was es im Clan darf.

Die maximale Anzahl von Mitgliedern des Clans ist abhängig vom [Rang des Clan-Leiters](../befehlsuebersicht/rang-befehle.md) und kann mit [speziellen Items](https://items.griefergames.net/#Rechte_%7C_%2B1_Clanmitglied) zusätzlich erhöht werden.

{% hint style="info" %}
Jeder Spieler kann einen Clan für 5.000.000$ erstellen. Bei der Auflösung eines Clans werden 2.000.000$ (40 % der Kosten) an den Clan-Leiter zurückerstattet. Das Guthaben der Clan-Bank erhält der Clan-Leiter ebenfalls.
{% endhint %}

{% hint style="warning" %}
Sonderrechte (bspw. zusätzliche Clan-Mitglieder, Clan-Farbcodes, Clan-Sondercodes) zählen nur, wenn der Clan-Leiter diese genutzt hat.
{% endhint %}

## Das Clan-Menü

Bist du in einem Clan, öffnet `/clan` das Menü **Dein Clan**. Dort findest du:

* **Clan-Name und Clan-Tag** deines Clans.
* **Mitglieder:** Alle Mitglieder mit ihrer Rolle und dem Server, auf dem sie gerade online sind. Außerdem siehst du, wie viele Plätze im Clan noch frei sind. Mit einem Klick auf ein Mitglied kannst du ihm eine Rolle geben oder es aus dem Clan werfen, sofern deine Rolle das erlaubt.
* **Clan-Homes:** Mit einem Linksklick teleportierst du dich zum Clan-Home. Mit einem Rechtsklick änderst du das Anzeige-Item, sofern deine Rolle Homes erstellen darf.
* **Einstellungen:** Hier ändert der Clan-Leiter den Clan-Namen und den Clan-Tag und verwaltet die Clan-Rollen.

## Clan-Rollen

Jeder Clan startet mit den Rollen **Clan-Leader**, **Clan-Moderator** und **Clan-Member**. Neue Mitglieder erhalten die unterste Rolle.

Der Clan-Leiter kann in den Einstellungen unter „Rollen bearbeiten“ eigene Rollen erstellen, umbenennen, sortieren und löschen. Für jede Rolle legt er fest, welche Rechte sie hat:

* Geld von der Clan-Bank abheben
* Homes erstellen und Icons ändern
* Homes löschen
* Rollen vergeben
* Spieler aus dem Clan kicken
* Spieler in den Clan einladen

Standardmäßig darf ein Clan-Moderator Homes erstellen und löschen sowie Spieler einladen und kicken. Rollen vergeben und Geld abheben darf zu Beginn nur der Clan-Leiter.

{% hint style="info" %}
Die Rolle Clan-Leader kann nicht bearbeitet werden. Gibst du als Clan-Leiter einem Mitglied diese Rolle, z. B. mit `/clan set <Spieler> Clan-Leader`, überträgst du ihm deinen Clan. Das ist nur alle **7 Tage** möglich.
{% endhint %}

## Clan-Befehle

| Befehl | Erklärung | Bilder |
| --- | --- | --- |
| `/clan create <Clan-Name> <Clan-Tag>` | <p>Damit legt man den Clan-Namen und den Clan-Tag fest, welcher im Chat steht.</p><p><strong>Wichtig:</strong> Der Clan-Tag muss zwischen 2 und 6 Zeichen lang sein. Eine Clan-Erstellung kostet 5.000.000$.</p> | <p><img src="../../.gitbook/assets/image (142).png" alt=""><br><img src="../../.gitbook/assets/image (143).png" alt=""></p> |
| `/clan settag <Clan-Tag>` | <p>Damit kann man den Clan-Tag bearbeiten, welcher 2-6 Zeichen lang sein darf.<br>Um einen Clan-Tag farbig zu gestalten, braucht man das Sonderrecht <a href="https://items.griefergames.net/#Rechte_%7C_BUNTE-Clan-Tags!">„Bunte Clan Tags“</a>. Falls man den Clan-Tag formatiert gestalten will, braucht man das Sonderrecht <a href="https://items.griefergames.net/#Rechte_%7C_Clan_Sondercodes">„Clan Sondercodes“</a> (bspw. magische Schrift).</p> | <p><img src="../../.gitbook/assets/image (146).png" alt="" data-size="original"><br><img src="../../.gitbook/assets/image (150).png" alt=""><br><img src="../../.gitbook/assets/image (151).png" alt=""></p> |
| `/clan setname <Clan-Name>` | Damit setzt man den Clan-Namen, welcher 2 bis 32 Zeichen lang sein darf. Clan-Name und Clan-Tag lassen sich jeweils nur alle 14 Tage ändern. |  |
| `/clan setcb <CB>` | Damit setzt man den Haupt-Citybuild-Server des Clans, welcher in der Clan-Information zu sehen ist. |  |
| `/clan sethome <Name>` | Setzt ein neues Clan-Home. |  |
| `/clan delhome <Name>` | Löscht ein Clan-Home. |  |
| `/clan home <Name>` | Teleportiert dich zum Clan-Home. |  |
| `/clan homes` | Listet aktuelle Clan-Homes auf. |  |
| `/clan invite <Spieler>` | Damit können Spieler, die keinen Clan haben, von Clan-Leitern und Clan-Moderatoren in den eigenen Clan eingeladen werden. |  |
| `/clan revoke <Spieler>` | Damit kann die Clan-Einladung, welche man verschickt hat, rückgängig gemacht werden. |  |
| `/clan invites` | Zeigt alle aktuellen Clan-Einladungen an. |  |
| `/clan list` | <p>Mit diesem Befehl werden alle Spieler im Clan angezeigt.<br>Zuerst der Clan-Leiter, dann die festgelegten Rollen und zuletzt die einfachen Clan-Mitglieder.</p> |  |
| `/clan roles` | Listet alle vorhandenen Clan-Rollen auf. |  |
| `/clan set <Spieler> <Rolle>` | Weist dem angegebenen Clan-Mitglied die gewünschte Rolle innerhalb des Clans zu. |  |
| `/clan info <Clan-Name/-Tag>` | Damit wird eine Clan-Übersicht des Clans angezeigt. |  |
| `/clan maxmember` | Zeigt an, wie viele Mitglieder der Clan insgesamt haben darf. | <img src="../../.gitbook/assets/image (149).png" alt="" data-size="original"> |
| `/cc` oder `/clanchat` | <p>Schreibe im Clan-Chat.<br>Nur für Clan-Mitglieder sichtbar und geht nicht im normalen Chat unter.</p> |  |
| `/clan guthaben` | Zeigt das aktuelle Guthaben in der Clan-Bank an. |  |
| `/clan einzahlen` | Geld in die Clan-Bank einzahlen. |  |
| `/clan abheben` | Geld aus der Clan-Bank abheben. |  |
| `/clan moneylog` | Geldverlauf der Clan-Bank anzeigen. |  |
| `/clan money` | <p>Zeigt das Clan-Geld an, sofern es aktiviert ist.<br>Das Clan-Geld ist die Summe der Vermögen aller Clan-Mitglieder.</p> |  |
| `/clan toplist` | Listet die reichsten Clans auf dem 1.8-Netzwerk auf. |  |
| `/clan togglemoney` | Aktiviert/Deaktiviert die Anzeige des Clan-Geldes, welches man unter <code>/clan money</code> sieht. |  |
| `/clan accept <Clan-Name>` | Damit kann man eine ausstehende Clan-Anfrage annehmen. |  |
| `/clan reject <Clan-Name>` | Damit kann man eine ausstehende Clan-Anfrage ablehnen. |  |
| `/clan kick <Spieler>` | Damit kann der Clan-Leiter oder Clan-Moderator ein Clan-Mitglied aus dem Clan werfen. |  |
| `/clan leave` | <p>Mit diesem Befehl kann man seinen aktuellen Clan verlassen.<br>Dies geht allerdings nicht als Clan-Leiter.</p> | <img src="../../.gitbook/assets/image (145).png" alt="" data-size="original"> |
| `/clan delete` | Damit kann der Clan-Leiter seinen Clan löschen. Die Löschung muss mit `/clan delete confirm` bestätigt werden und kann nicht rückgängig gemacht werden. | <p><img src="../../.gitbook/assets/image (147).png" alt="" data-size="original"><br><img src="../../.gitbook/assets/image (148).png" alt=""></p> |

{% hint style="info" %}
Ein Clan wird nicht von der Administration übertragen. Bereits vergebene Clan-Namen werden nicht neu vergeben.
{% endhint %}
