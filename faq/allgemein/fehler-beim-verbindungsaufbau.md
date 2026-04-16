---
description: io.netty.channel / connection timed out / sending too many packets
---

# Fehler beim Verbindungsaufbau

## Vorwort: Datenverkehr - Warum passiert das?

Eine Anfrage im Internet zwischen deinem Endgerät und einem Server wird in einzelne Datenpakete zerlegt. Diese Pakete enthalten Informationen zu ihrem Ursprung, ihrem Ziel, ihrer Art von Verarbeitung, sowie die reinen Daten-Informationen, welche eigentlich gesendet werden. Da pro Paket immer nur eine gewisse Größe möglich ist werden umfangreichere Anfragen in eine Vielzahl an Paketen zerlegt und am Ziel wieder zusammengesetzt.

Gehen hierbei Datenpakete verloren oder werden unterwegs im Netz "beschädigt" (fehlerhaft gelesen, geschrieben, übertragen), muss dieses vom Ziel entweder auf Grundlage von anderen Datenpaketen repariert werden (FEC-Fehler) oder komplett neu vom Ursprung angefordert werden (CRC-/CV-Fehler).

Beachte hierbei, dass eine **schnelle** Internetverbindung nicht gleichzeitig eine **stabile** Internetverbindung bedeutet.

* Eine hohe Bandbreite heißt nur, dass viele Datenpakete in kurzer Zeit transportiert werden.
* Die Latenz sagt nur aus, wie lange das Datenpaket für die Übermittlung zum Server benötigt hat.
  * Eine zu hohe Latenz führt potentiell häufiger zu timeout-Fehlern oder ist Ursache für einen Packet-Spam.
* Die Qualität wird dadurch bestimmt, wie viele der gesendeten Datenpakete unbeschädigt ankommen bzw. FEC-seitig reparierbar sind.
  * Zu viele FEC oder CRC-Fehler führen zu einer beeinträchtigten Verbindung.

### Was ist ein "io.netty.channel"-Fehler?

Wie alle Fehlermeldungen besteht diese aus mehreren technischen Teilen:

* `io` = I/O = Input-Output, typischer Informationsfluss in der Computertechnik (Eingabe-Ausgabe-Verfahren, Anfrage-Antwort, Server-Client, etc.)
* netty = API-Name ([Mehr Informationen](https://netty.io/4.0/api/overview-summary.html))
* `netty.channel` = Kernkanal-API zur asynchronen und ereignisgesteuerten Abstraktion verschiedener Transporte

**"io.netty.channel"**-Fehler treten in Minecraft auf, wenn die verwendete Kern-API für das Verbinden der Client-Anfrage in Richtung Server scheitert. Im Normalfall passiert das, weil der Client keine bzw. unzureichende oder fehlerhafte Daten liefert.

Dies kann verschiedene Ursachen haben, welche in diesem Eintrag behandelt werden. Die Ursachen sind dabei nicht für jeden Fehler exklusiv, sondern können zu jedem dieser Fehler beitragen oder andere Fehlerquellen "verschlimmern".

### Was ist ein Timeout?

Bei einem Timeout sendet dein Client eine Anfrage an den Server. Dein Endgerät erwartet, dass der Server diese Anfrage innerhalb einer gewissen Zeit beantwortet. Bleibt die Antwort über einen gewissen Zeitraum hinweg aus, trennt das System die Verbindung mit der Meldung **"timed out"**, zu deutsch "Zeitüberschreitung". Die erwartete Zeit für eine Antwort ist überschritten. Die Verbindung wird getrennt, da keine Antwort erfolgt ist und das System davon ausgeht, dass das Ziel nicht antwortet.

Dieser Vorgang kann selbstverständlich auch umgekehrt erfolgen. Sendet der Server eine Anfrage an deinen Client und diese wird nicht beantwortet, trennt der Server die Verbindung, da er davon ausgeht, dass dein Client nicht mehr verbunden ist. Üblicherweise erfolgt dies mit einer Fehlermeldung, welche aussagt, dass **der Remotehost die Verbindung getrennt hat**.

### Was ist ein Packet-Spam?

Wenn der Server eine unnormale Vielzahl von Datenpaketen von deinem Client auf einmal erhält, interpretiert der Server dies als Versuch ihn zu "überfordern" oder gar als "Angriff" und trennt die Verbindung zu dir, um sich zu schützen. Du erhältst eine Fehlermeldung mit dem Inhalt **"packet spam"** oder **"sending too many packets"**, zu Deutsch "sendet zu viele Pakete".

Ein Packet-Spam ist daher so ziemlich das Gegenteil vom "timeout"-Fehler, hat aber in der Regel die gleiche grundlegende Ursache: _Das von deinem Client gesendete Signal benötigt "zu lange" um beim Server anzukommen._ In den meisten Fällen liegt irgendwo ein "Flaschenhals", welcher das Signal ausbremst und die Datenpakete zwischen deinem Client und dem Server aufhält. Sobald die Datenpakete die "Blockade" überwunden haben oder diese sich auflöst, werden diese alle auf einmal gesendet.

## Was kann ich nun tun? Mögliche Fehlerbehebung

### **Generelle io.netty.channel-Probleme:**

* **Java veraltet**
  * Der Minecraft-Launcher kommt standardmäßig mit einer eigenen Java-Instanz, welche mit Client-Updates auch aktualisiert wird. Manchmal ist diese dennoch veraltet oder fehlerhaft. Hier hilft es dann im Launcher unter Installationen > Bearbeiten > Mehr Optionen eine aktuelle Java-Instanz vom eigenen PC zu nutzen.
  * Java kann in der Systemsteuerung deines Betriebssystems aktualisiert werden. Falls du Java noch nicht seperat installiert hast, kannst du dir einen Installer von der [offiziellen Webseite herunterladen](https://www.java.com/de/download/).
* Benutzt du die **passende Minecraft-Version** für den Server?
  * Für das optimale Spielen auf GrieferGames.net "Citybuild 1.8" wird Minecraft 1.8.9 empfohlen!
  * Für das optimale Spielern auf GrieferGames.net "Citybuild Cloud" wird die aktuelle Minecraft-Version empfohlen!
* Benutzt du die aktuelle **Minecraft-Version für Bedrock**?
  * Du kannst den Softwarestand über den entsprechenden Store des Endgerätes prüfen.
  * Die Beta-Versionen der App werden **nicht** unterstützt!

### **Timeout- & Packet-Spam-Probleme:**

* Verbindest du dich auf **GrieferGames** über <kbd>griefergames.net</kbd>?
  * Viele unserer Alternativadressen wurden inzwischen **deaktiviert**.
  * Für das Verbinden auf unsere Server empfehlen wir die Adresse "griefergames.net".
    * Die Alternative für die Java-Edition ist: <kbd>alt.griefergames.net</kbd>
    * Die Alternativadresse <kbd>cloud.griefergames.net</kbd> kann direkt auf unser [Cloud-Netzwerk](https://app.gitbook.com/o/nS9KOXaVZVX5hWgLD6av/s/i10PgHQTIUUm2awhkL0L/) verbinden. Du benötigst hierfür **mindestens** den [Premium-Rang](../../grundlagen/befehlsuebersicht/rang-befehle.md#premium).
    * Für die Bedrock-Edition bestehen keine Alternativ-Adressen. _(siehe hierzu Firewall-/Port-Einstellungen)_
* Spielst du über einen **VPN/Proxy/festen DNS-Server**, welcher deine Daten "umleitet"?
  * Versuch einen direkten Verbindungsaufbau ohne "Zwischenstopp", um einen Fehler bei diesem auszuschließen.
  * Derlei Dienste gibt es auch für mobile Endgeräte. Manchmal sind diese sogar bordseitig aktiv.
* Benutzt du **Sicherheitssoftware** (Antivirus/Malware/Sicherheitspakete)?
  * Die entsprechenden Programme durchsuchen den Datenverkehr der Netzwerkverbindung, um potentielle Bedrohungen aufzuspüren. Der Datenverkehr wird dafür kurzzeitig angehalten und in der Software geprüft, was zu einer Verzögerung führen kann.
* Bitte überprüfe, dass deine **Firewall** nicht den Minecraft-Port '25565' und den Bedrock-Port '19132' über TCP und UDP blockiert hat.
  * Wie du das am Besten machst, erfährst du durch eine Recherche auf Google oder in Rücksprache mit dem Hersteller-Support des Gerätes bzw. der Software.
  * Die Alternativports der Java-Edition sind 25566 und 25567.\
    Für eine optimale Freigabe ist daher der Bereich <kbd>25565 - 25567</kbd> auf TCP und UPD freigegeben.
  * Der Alternativport der Bedrock-Edition ist 19134.\
    Für eine optimale Freigabe ist daher der Bereich <kbd>19132, 19134</kbd> auf TCP und UDP freigegeben.
* Wenn du die Bedrock-Edition verwendest kann das **Ändern von Einstellungen** den Datenverkehr reduzieren und damit die Qualität verbessern (weniger Datenbelastung). Hierfür nutzt du auf unserem Server das Menü > Einstellungen und den Befehl `/settings`.

Ein weiterer Faktor neben diesen typischen "Flaschenhälsen" sind natürlich auch die **eigene Internetverbindung** und die Latenz zwischen Server und Client.

* Für eine **stabile** Internetverbindung ist eine Bandbreite von mehr als 6 MBit/s im Downstream und 2 MBit/s im Upstream erforderlich. Ich **empfehle** eine Bandbreite von mindestens 16 MBit/s im Downstream und 6 MBit/s im Upstream.
  * Die genaue Bandbreite des Anschluss lässt sich über das Menü eures Routers ermitteln. In der Statusübersicht werden die Werte normalerweise angegeben.
  * Alternativ könnt ihr jederzeit eine Prüfung des Anschluss durch euren Anbieter veranlassen.
* Die **Latenz** beschreibt die Dauer die das Signal zwischen Client und Server und zurück benötigt. Sie wird auch als "ping" bezeichnet.
  * Werte von 10-25 ms sind optimal für einen Verbindungsaufbau.
  * Pingzeiten bis zu 50 ms sind verträglich, alles darüber wird unangenehm.
  * Die Latenz sollte in keinem Fall über 100ms liegen.
* "LAN-Ersatzlösungen", wie WLAN-Verbindungen, Powerline-Verbindungen oder USB-Tethering verzögern den Verbindungsaufbau und den Paketdurchsatz. Solche **Verbindungsarten im Heimnetz** können ebenfalls zum "Stau" der Datenpakete führen.
  * Teste die Verbindung zeitweise mit einer mobilen Datenverbindung.
  * Entferne andere Geräte vom Router oder deaktiviere deren WLAN-Verbindung für die Dauer deines Tests, um Einflüsse aus deinem Heimnetzwerk zu verhindern.
* Dienste wie IPTV oder VoIP haben bei fast allen Anbietern eine **"QoS"-Priorisierung**.
  * Telefoniert also jemand in eurem Heimnetzwerk oder schaut über das Internet Fernsehen, so ist dieser Datenverkehr bevorzugt und eurer wird "hinten angestellt".
* Mobile Daten werden über die Mobilfunk-Anbieter nach einem **"shared medium"-Prinzip** ausgegeben.
  * Die Verbindungsqualität schwankt daher abhängig der aktuell an der Funkzelle verbundenen Nutzer und deren Nutzungsverhalten.
  * Teste ggf. die Verbindung über das Netzwerk des Routers.

Eine letzte Möglichkeit ist natürlich auch serverseitig zu finden und das sind "Lag-Spikes" des Servers.

Ist der Server gerade durch zu viele Anfragen ausgelastet _(wie bei DDoS-Angriffen/Hoster-Problemen)_, dauert es ebenfalls einen kurzen Moment bis deine Datenpakete verarbeitet werden. Wenn diese sich in der Zeit "anstauen" kann dies ebenfalls als "Paket-Spam" interpretiert und du vom Server geworfen werden.

Aktuelle Informationen zur Serverperformance findest du auf [unserem Discord](https://discord.griefergames.net/).



{% hint style="warning" %}
Die Kombination aus zwei oder mehr dieser Punkte sorgt natürlich für ein höheres Fehlerpotential. Es kann also sein, dass alle einzelnen Bedingungen in Ordnung sind und eine ping-Zeit von 45 ms in Kombination mit einer Nutzung der mobilen Daten und aktuellen Hoster-Problemen dennoch zum Fehler führt.
{% endhint %}

<details>

<summary>An diesem Artikel beteiligt</summary>

* [50U7R34P3R](https://profile.griefergames.live/minecraft/8e2ce0be-aa2c-46a7-a2dc-48f948743edf)

</details>
