---
description: Hier findest du Antworten auf typische Anliegen zu unserem TeamSpeak-Server
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

# TeamSpeak

### TeamSpeak: Minecraft-Rang synchronisieren

Wenn du deinen Minecraft-Rang auch auf unserem TeamSpeak-Server haben willst, musst du dich auf dem TeamSpeak-Server genau so nennen wie in Minecraft, damit unser Bot dich erkennen kann.

Wenn du dies getan hast, musst du dich auf unserem TeamSpeak-Server in der Eingangshalle befinden.

Danach kannst du in der Lobby (`/hub`) unseres Minecraft-Servers einen der Befehle

* `/ts update`
* `/ts`
* `/tsu`
* `/teamspeak`
* `/teamspeakupdate`&#x20;

eingeben. Jetzt musst du nur noch einige Sekunden bis wenige Minuten warten.

Falls die Rang-Synchronisierung nicht funktionieren sollte, versuche es nach 24 Stunden erneut. Der Bot ist nicht zu 100% fehlerfrei und legt ab und zu eine kleine „Ruhezeit“ ein.

Sollte auch nach 24 Stunden keine Synchronisation deines Ranges möglich sein, wende dich bitte an ein Teammitglied.



### TeamSpeak: Forum-Verifikation

Für die volle Funktion des TeamSpeak-Servers wird immer eine Verifikation benötigt.

Hierzu können Gäste ihre TeamSpeak-Identität mit einem existierenden Foren-Account verknüpfen, auch wenn dieser keinen Minecraft-Account verknüpft hat.

{% hint style="info" %}
Die Erstellung eines neuen Foren-Accounts ist nur noch über GGAuth möglich. Hierfür wird ein beliebiger Minecraft-Account benötigt. Ohne einen Minecraft-Account ist keine Verifikation auf dem TeamSpeak-Server mehr möglich.
{% endhint %}



**Ablauf der Verifikation**

1. Anmeldung mit einem existierenden GGAuth-Account
2. nach unten scrollen zu "Account-Verknüpfungen"&#x20;
3. In der Kachel Teamspeak den Button „Verknüpfung hinzufügen“ anklicken
4. Die eindeutige ID eintragen\*\* und bestätigen
5. Folge den Anweisungen auf der Accountverwaltung, bis der Vorgang erfolgreich abgeschlossen ist.
6. Das System verifiziert dich und du hast ab sofort die entsprechende Gruppe und Rechte auf unserem TeamSpeak-Server.

{% hint style="warning" %}
Du kannst in deinem GGAuth-Account immer nur **eine e**indeutige Identität verknüpfen.
{% endhint %}

{% hint style="info" %}
Die eindeutige ID findest du im TeamSpeak-Client unter _Extras_ » _Identitäten_ (Expertenmodus aktiviert)
{% endhint %}



Für noch mehr Austausch (ohne Minecraft-Account) schau auch gerne auf unserem [Discord-Server](https://discord.griefergames.net/) vorbei.



### TeamSpeak: Anstupsen deaktivieren

Du kannst selbst entscheiden, wie du das deaktivieren möchte. Hierzu gibt es zwei Möglichkeiten:\
(Natürlich kannst du auch beide ausführen)

#### Anstupser-Sound deaktivieren

Wenn du den Sound des Anstupsen deaktivieren möchtest, dann musst du folgenden Weg gehen (TeamSpeak-Version 3):

1. In der Menüleiste „Extras“ anklicken
2. Dann auf „Optionen“ klicken
3. Folgend mit dem Klick auf „Meldungen“
4. Jetzt musst du den Sound finden. Dafür gehst du auf „Andere“.
5. Nun siehst du einige Einträge, u.a. auch „Anstupsen empfangen“ – den Haken aus der Checkbox nehmen und fertig – den Sound von einem Anstupser hörst du nun nicht mehr.

#### Anstupser-Benachrichtigung als Pop-up deaktivieren

Wenn du die Benachrichtigung des Anstupsens nicht mehr als Pop-up Fenster sehen möchtest, kannst du den Anstupser zwar nicht komplett deaktivieren, jedoch zum Teil. Du erhältst die Meldung weiterhin als normale Nachricht im Channel-Chat, in welchem du dich aufhältst. Um dies einzustellen, musst du folgendem Weg folgen (TeamSpeak-Version: 3):

1. In der Menüleiste „Extras“ anklicken
2. Dann auf „Optionen“ klicken
3. Folgend mit dem Klick auf „Anwendung“
4. Jetzt musst du nur noch in der Unterkategorie „Verschiedenes“ den Haken in der Checkbox „Anstupsen Dialog nie zeigen“ setzen und fertig!



### TeamSpeak: Mikro-Qualität & Echo

#### **Andere Personen im Channel hören sich selbst über dein Mikrofon! Wie kannst du dieses Problem lösen?**

Wenn du dich mit einem Endgerät ohne Headset (Lautsprecher und Mikrofon) auf dem TeamSpeak-Server verbindest, kann es sein, dass andere Personen im Channel sich selbst über dein Mikrofon hören können.

Das Problem kann gelöst werden, indem du ein Headset anschließt, Push-to-Talk benutzst oder einfach die Sensibilität der Sprachaktivierung anpasst.&#x20;

Das Erhöhen der Sensibilität stellt jedoch ein Problem dar. Du musst höchstwahrscheinlich sehr laut sprechen, damit die anderen Personen im Channel dich hören können.&#x20;

Die sinnvollste Methode, wenn du kein Headset hast oder benutzen möchtest ist daher "**Push-to-Talk"**.

Push-to-Talk ermöglicht es dir, wenn du eine Taste auf der Tastatur oder eine Makrotaste auf deiner Maus drückst, dein Mikro freizuschalten. Beim Loslassen der Taste wird das Mikro gesperrt und andere Personen können dich nicht mehr hören.

#### **Konfiguration Push-to-Talk (TeamSpeak 3)**

Navigiere oben in der Menüleiste auf „Extras“. Dort steht ganz unten „Optionen“ – klicken und zu „Aufnahme“ gehen. Dort wählst nun den Aufnahmemodus („Automatisch besten Modus wählen“ empfehlenswert) und dein Aufnahmegerät (Mikrofon) aus.

Jetzt siehst du drei Möglichkeiten, die Aufnahme zu konfigurieren: **Push-to-Talk**, **Dauersenden** (nicht empfehlenswert) und **Sprachaktivierung**.

Nun klicke den "RadioButton" bei Push-to-Talk an, sodass diese ausgefüllt ist. Jetzt nur noch die Taste auswählen, indem du auf „Kein Hotkey zugewiesen“ klickst und die Taste betätigst, die du für PTT verwenden willst. Zudem kannst du noch die Checkbox bei „Echo Abschwächung“ setzen und bei „Erweiterte Optionen“ das Feature „Hintergrundgeräusche entfernen“ aktivieren. Das sorgt für ein klareres Klangerlebnis und fokussiert deine Stimme.

Falls du keine Verzögerung beim Sprechen haben willst, wenn du Push-to-Talk benutzt, dann gebe bei „Verzögerung Push-to-Talk“ in das Feld „0,1 Sek“ ein.

Jetzt nur noch auf „Anwenden“ klicken und fertig.

Das Ganze sollte nun so aussehen:

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Empfohlene Einstellungen für Push-to-Talk in TeamSpeak 3</p></figcaption></figure>

Es gibt natürlich noch weitere Möglichkeiten, die Qualität deiner Audioverbindung zu verbessern. Du kannst dir ein qualitativ hochwertiges Mikrofon (und Mischpult) zulegen oder einfach VoiceMeeter benutzen. Diese Software ist ein virtuelles Mischpult und bietet grandiose Einstellungen. \
Wie du diese Software installierst und einstellst, erfährst du durch Tutorials auf YouTube.
