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

# 💬 Das Chat-System

Auf dem Server kannst du auf verschiedene Arten mit deinen Mitspielern schreiben.

Eine Übersicht aller Möglichkeiten findest du hier in diesem Artikel.

### Chat-Codes

Im Chat können verschiedene Codes verwendet werden, um Nachrichten farbig darzustellen oder zu formatieren. Dazu wird der jeweilige Code vor den gewünschten Text gesetzt.

Bei der Nachricht "Ich verkaufe mein Grundstück" in grüner Farbe würde das dann bevor du es in den Chat abschickst so aussehen:

<figure><img src="../.gitbook/assets/AdXK2Os.png" alt=""><figcaption></figcaption></figure>

Eine Übersicht aller Chat-Codes (Farben, Formatierungen) findest du hier:

<table><thead><tr><th>Code</th><th>Farbe / Effekt</th><th data-hidden></th></tr></thead><tbody><tr><td>&#x26;0</td><td>Schwarz</td><td></td></tr><tr><td>&#x26;1</td><td>Dunkelblau</td><td></td></tr><tr><td>&#x26;2</td><td>Dunkelgrün</td><td></td></tr><tr><td>&#x26;3</td><td>Dunkelcyan</td><td></td></tr><tr><td>&#x26;4</td><td>Dunkelrot</td><td></td></tr><tr><td>&#x26;5</td><td>Dunkellila</td><td></td></tr><tr><td>&#x26;6</td><td>Gold</td><td></td></tr><tr><td>&#x26;7</td><td>Grau</td><td></td></tr><tr><td>&#x26;8</td><td>Dunkelgrau</td><td></td></tr><tr><td>&#x26;9</td><td>Blau</td><td></td></tr><tr><td>&#x26;a</td><td>Grün</td><td></td></tr><tr><td>&#x26;b</td><td>Cyan</td><td></td></tr><tr><td>&#x26;c</td><td>Rot</td><td></td></tr><tr><td>&#x26;d</td><td>Pink</td><td></td></tr><tr><td>&#x26;e</td><td>Gelb</td><td></td></tr><tr><td>&#x26;f</td><td>Weiß</td><td></td></tr><tr><td>&#x26;k</td><td>Zufallstext / Wechselnde Zeichen</td><td></td></tr><tr><td>&#x26;l</td><td>Fett</td><td></td></tr><tr><td>&#x26;m</td><td>Durchgestrichen</td><td></td></tr><tr><td>&#x26;n</td><td>Unterstrichen</td><td></td></tr><tr><td>&#x26;o</td><td>Kursiv</td><td></td></tr></tbody></table>

### Öffentlicher Chat

Der öffentliche Chat ist der Chat, in dem du schreibst, wenn du auf einem [Citybuild-Server](../grundlagen/spielmodus-citybuild/) bist. Dieser Chat kann von jedem Spieler auf diesem Citybuild gelesen werden, welcher gerade online ist.&#x20;

Die Chatteilnehmer hängen hier von der Anzahl an Spielern an, die gerade auf dem Citybuild-Server anwesend sind.&#x20;

Solltest du also auf einem Citybuild-Server sein, auf welchem nur um die 10 Spieler online sind, so können nur wenige Spieler auf deine Nachrichten antworten, da die Nachrichten nur von wenigen Spielern gelesen werden.&#x20;

Auf volleren Citybuilds können mehr Spieler deine Nachricht lesen. Hier gibt es dann aber den Nachteil, dass auch mehr Nachrichten in den Chat geschrieben werden und deine Nachricht schneller überlesen werden kann.

### Globaler Chat

Der globale Chat ist eine neue Art des Chats, mit dem du mit Spielern auf anderen Citybuilds schreiben kannst. Hierbei kannst du aber nur mit Spielern schreiben, die in den Chat eingeloggt sind.

Um dich im Globalchat anzumelden, musst du den Befehl `/globalchat login` eingeben. Nun siehst du neben den Nachrichten aus dem öffentlichen Chat auch die Nachrichten von Spielern von anderen Citybuilds.&#x20;

Diese Nachrichten erkennst du daran, dass vor dem Spielernamen ein @ steht und dahinter der Citybuild in Klammern.

<figure><img src="https://lh6.googleusercontent.com/W5z7F1MgVd_aEZtw6LR4hRzAP8QihRpYRc3OCnWTKxbGYqaVHoZRcyEkmBY__95jWeb6P7393PnpOPP_eEBkXd8LmFVxj9-c3txV2y4VpyAdSRKXJTkqCT1gJIz92eC9ygDeQv7tTaSNWoxLA5MKNHM" alt=""><figcaption><p>Nachricht eines Spielers im Globalen Chat zwischen Nachrichten iom Öffentlichen Chat</p></figcaption></figure>

Um eine Nachricht in den globalen Chat zu schreiben, kannst du dies zum einen mit `/globalchat <Nachricht>` machen. Wir empfehlen die Verwendung des Kurzbefehls `@<Nachricht>`.&#x20;

{% hint style="warning" %}
Vergiss nicht, dass du dafür in den Globalen Chat angemeldet sein musst.
{% endhint %}

Du kannst unter `/globalchat settings` einstellen, von welchen Citybuilds du keine Nachrichten erhalten möchtest.

Wenn du nun keine Nachrichten aus dem GlobalChat mehr sehen möchtest, kannst du dich mit `/globalchat logout` aus dem globalen Chat abmelden.

### Plot-Chat

Der Grundstückschat (auch _Plot-Chat_ genannt) ist ein Chat, bei welchem nur die Mitspieler auf einem [Grundstück](../grundlagen/grundstuecke/) die geschriebenen Nachrichten lesen und auf diese antworten können.

Hierfür musst du auf einem Grundstück stehen und den Plot-Chat mit `/p chat` aktivieren. Alle von dir darauf folgenden Nachrichten werden nun in den Plot-Chat geschrieben.

Alle Nachrichten aus dem Grundstückschat haben vor dem Spielernamen in Klammern, dass diese aus dem Plot-Chat sind und auf welchem Grundstück (ID) die Nachrichten geschrieben werden.

Um den Plot-Chat wieder zu deaktivieren, musst du den selben Befehl `/p chat` noch einmal eingeben. Hierbei steht dann auch immer im Chat, ob der Plot-Chat aktiviert oder deaktiviert ist.

<figure><img src="https://lh6.googleusercontent.com/ZbtpZbfQswnVxjfn4znB2s-x4b9Bf1v5peBKbyh4uIulV1OEZLYnwm73MYTF2dfAEp1vZts0DTy8Thgn4eaZCZjSxJOWN1YGbASCJn4nfIPXgJFRWURT2O9uIMCKhjwDq9IlUZ8rhwPEK84wBDJS4H8" alt=""><figcaption><p>Aktivierungsbestätigung, eine Nachricht im Plot-Chat und Deaktivierungsbestätigung</p></figcaption></figure>

### Privater Chat

Zum Handeln oder allgemein braucht man gelegentlich die Funktion, mit einem Spieler privat zu schreiben. Dafür gibt es private Nachrichten.

Mit `/msg <Spieler> <Nachricht>` kannst du mit jedem Spieler auf dem Citybuild-Server privat schreiben.

Das heißt, dass nur dieser Spieler die Nachricht sieht.\
Dieser Spieler kann dir dann auf dieselbe Weise wieder eine Nachricht zurück schreiben.

Mit dem Befehl `/r <Nachricht>` antwortest du der letzten Person, mit welcher du privat geschrieben hast, direkt. In Handelsgesprächen ist dies meist einfacher, da du nicht so einen langen Befehl eintippen musst.

{% hint style="warning" %}
Sollte dich in der Zeit aber ein anderer Spieler anschreiben, da du vielleicht mit zwei Spielern gleichzeitig schreibst, bekommt dieser Spieler die Nachricht, da dieser Spieler die letzte Person ist, welche mit dir privat geschrieben hat.
{% endhint %}

<figure><img src="https://lh4.googleusercontent.com/cnhD8I6GtM9Gjl3ecmFG6Bf8O0T2QCYxJ58nxjkcJ5SKl391Kjw6rleOTfkL5vPdqVBuM06wzOVmlp19qHN3XHvyfnX0Xuc6ojw9auwzzy0r-sIt9ZyWA_PsNFuRvmwjmNP6w-K4MR4atUIhi3xhx8w" alt=""><figcaption><p>Direktnachrichten zwischen 2 Spielern</p></figcaption></figure>

Die Nachrichten werden anders angezeigt, je nachdem ob du die Nachricht versendet hast oder ob du sie erhältst.

Wenn du eine Nachricht sendest steht da, dass die Nachricht von dir zu einem Empfänger geht `[mir -> Empfänger]`. Andersrum kommt die Nachricht vom Absender zu dir `[Absender -> mir]`.

Falls du nicht direkt angeschrieben werden willst, kannst du dies im Profil-System `/profil` einstellen. Dies steht allen Accounts zur Verfügung, welche einen Rang haben ([Premium](../grundlagen/befehlsuebersicht/rang-befehle.md#premium) und höher).

Dafür musst du Folgendes machen: `/profil` -> Einstellungen -> Private Nachrichten -> Auf die Glasscheibe klicken.

<figure><img src="https://lh4.googleusercontent.com/HOwBWiz6DzygMBUMNrFrnZKCNwSoC9J4WlfAspNO6Vab5jaGeb9KftKY-EC89S4U2PT-HY5284KLV919iMlm-1VqKQ-Sk7FiN5Of627CkPCpUcCQlK0y0ZQdMP4ShVNklCwQ7xxhRHMFDUHlRudzHOE" alt=""><figcaption><p>Einstellungen im Profil-System</p></figcaption></figure>

Wenn du Direktnachrichten deaktiviert hast, kannst du zwar nicht angeschrieben werden, aber andere Spieler anschreiben. Diese können dir aber nicht per Direktnachricht antworten.

{% hint style="info" %}
Die Funktion kann auch mit dem Befehl `/msgtoggle` umgeschaltet werden.
{% endhint %}

### Spieler ausblenden

Wenn dich die Nachrichten eines Spielers stören, kannst du diese auch ausblenden. Dafür gibst du einfach `/ignore <Spieler>` im Chat ein. Nun siehst du keine Chatnachrichten dieses Spielers mehr.&#x20;

Du siehst jedoch weitere Aktionen des Spielers (bspw. Statusnachricht, Abstimmungen, etc.)

Wenn du die Chat-Nachrichten des Spielers wieder sehen willst, gibst du den gleichen Befehl noch einmal ein.

Mit `/ignore` siehst du eine Liste von allen Spielern, welche du ignoriert hast.

### Chat-Sperren

Du kannst nicht im Chat schreiben und erhältst eine Fehlermeldung? \
Dafür kann es mehrere Gründe geben:

* Der Chat in den Chateinstellungen ist auf „Nur Befehle“ gestellt.
* Dein Account wurde durch ein Teammitglied/einen Spieler mit dem Mute-Perk gestummt.
* Man befindet sich in der Lobby oder im Portalraum, wo der Chat komplett deaktiviert ist.
* In deiner Nachricht befinden sich ein oder mehrere Wörter, die vom Team verboten wurden und somit auf die Blacklist gesetzt worden sind.
