---
description: Befehle, die das Plot betreffen
---

# Grundstücks-Befehle

### Grundstücke erhalten

| Befehl     | Funktion                                                                                                          |
| ---------- | ----------------------------------------------------------------------------------------------------------------- |
| /p auto    | Erhalte ein zufällig gewähltes freies Grundstück                                                                  |
| /p claim   | Erhalte das freie Grundstück, auf welchem du dich aktuell befindest                                               |
| /checkplot | [Grundstück eines inaktiven Spielers beantragen](../../grundstuecke/grundstuecke-inaktiver-spieler-beantragen.md) |

### Grundstücks-Teleport

| Befehl                                           | Funktion                                                                                                                                        |
| ------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| <p>/p h {Zahl}<br>/plot home {Zahl}</p>          | <p>Teleportiere dich zu deinem Grundstück<br></p><p>Beispiel: <code>/p h 2</code> bringt dich auf dein zweites Grundstück.</p>                  |
| <p>/p h {Spielername} {Zahl}<br>/p h {Alias}</p> | Teleportiert dich zum Grundstück eines Mitspielers.                                                                                             |
| /p middle                                        | Teleportiere dich zur Mitte des Grundstück                                                                                                      |
| <p>/p sethome<br>/p &#x3C;ID> sethome</p>        | [Versetze den Spawnpunkt](../../../faq/citybuild/grundstuecke-verwalten.md#grundstueck-unerreichbar) des Grundstücks an deine aktuelle Position |

### Grundstück verwalten

| Befehl                            | Funktion                                                                                                                                  |
| --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| <p>/p i<br>/plot info</p>         | Zeigt eine Übersicht mit [Informationen und Einstellungen des Grundstücks](grundstuecks-informationen.md) an                              |
| <p>/p<br>/plot<br>/m<br>/menu</p> | [Grundstücks-Menü](../../grundstuecke/grundstueck-menue.md) aufrufen                                                                      |
| /merge                            | [Grundstücke verbinden](../../grundstuecke/grundstuecke-verbinden.md)                                                                     |
| /mergebug                         | Fehler beim Verbinden an der aktuellen Position an das Team melden                                                                        |
| /p clear                          | <p>Grundstück in den Ursprungszustand versetzen <br></p><p><strong>Achtung!</strong> Bei einem Merge werden die Grundstücke getrennt!</p> |
| <p>/p delete<br>/p reset</p>      | Grundstück löschen und freigeben                                                                                                          |

### Rechte verwalten

Natürlich könnt ihr auch gemeinschaftlich an Projekten arbeiten. Dazu könnt ihr anderen Spielern Rechte zuweisen oder unerwünschten Besuch fernhalten.

| Befehl                   | Funktion                                                                                   |
| ------------------------ | ------------------------------------------------------------------------------------------ |
| /p trust \<Spielername>  | Der Spieler erhält volle Rechte auf deinem Grundstück und allem, was zum Grundstück gehört |
| /p add \<Spielername>    | Der Spieler verfügt nur über die Rechte, sofern du auf dem Citybuild online bist           |
| /p remove \<Spielername> | Du entziehst dem Spieler alle Rechte von deinem Grundstück                                 |
| /p deny \<Spielername>   | Der Spiele kann dein Grundstück nicht mehr betreten                                        |
| /p undeny \<Spielername> | Der Spieler darf dein Grundstück wieder betreten                                           |
| /p kick \<Spielername>   | Der Spieler wird von deinem Grundstück geworfen und kann direkt wieder drauf               |

Solltest du statt einem Spielernamen ein `*` einfügen, so gilt dieser Befehl für alle Spieler.

{% hint style="info" %}
`/p trust AbgegrieftHD` - Abge darf sich auf deinem Grundstück austoben. Sonst niemand.\
`/p trust *` - Jeder Anwesende kann auf deinem Grundstück alles machen.
{% endhint %}

{% hint style="danger" %}
Rechte für alle Spieler zu vergeben ist nicht sonderlich ratsam und nur bedingt zu empfehlen.
{% endhint %}

### Weitere Grundstücks-Befehle

| Befehl                                       | Funktion                                                                                                                                                                               |
| -------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| /setowner {Spielername}                      | Starte eine Überschreibung deines Grundstücks an einen anderen Spieler                                                                                                                 |
| /setowner confirm                            | Bestätige die Überschreibung eines Grundstück                                                                                                                                          |
| /setowner deny                               | Lehne die Überschreibung eines Grundstückes ab                                                                                                                                         |
| /p description {Text}                        | Füge deinem Grundstücke eine Beschreibung hinzu                                                                                                                                        |
| /p description                               | Entferne die Beschreibung des Grundstück                                                                                                                                               |
| /p alias set {Text}                          | <p>Gib dem Grundstück einen Namen (Alias)<br><br><strong>Achtung!</strong> Es können keine Namen von Spielern genutzt werden, welche bereits auf dem Server angemeldet sind/waren.</p> |
| <p>/p chat on<br>/p chat off</p>             | <p>Schreibe im Grundstücks-Chat<br>Schreibe im Normalchat</p>                                                                                                                          |
| /p flag set {Flag} {true/false/ID}           | [Grundstücks-Flag](grundstuecks-flags.md) setzen                                                                                                                                       |
| /p setorder {Zahl}                           | Setzt das Grundstück an die ausgewählte Position deiner Grundstücksliste                                                                                                               |
| /bewertung                                   | Aktiviere die Bewertungsfunktion für dein Grundstück                                                                                                                                   |
| /bewerten                                    | Menü zur Grundstücks-Bewertung aufrufen                                                                                                                                                |
| <p>/ptime {Zahl}<br>/ptime {Tageszeit}</p>   | Setze die aktuelle Zeit auf deinem Grundstück                                                                                                                                          |
| <p>/ptime @{Zahl}<br>/ptime @{Tageszeit}</p> | Setze die Zeit auf deinem Grundstück dauerhaft fest                                                                                                                                    |
| /leuchten                                    | <p>Leuchtfeuer an den Grundstücksecken platzieren<br><em>(Recht kann im CaseOpening gewonnen werden)</em></p>                                                                          |
| /rand                                        | Ändere den Grundstücksrand                                                                                                                                                             |
| /wand                                        | Ändere die Grundstückswände                                                                                                                                                            |
| /boden                                       | Ändere den Grundstücksboden                                                                                                                                                            |
| /aushöhlen                                   | Öffne das Menü zum Aushöhlen des Grundstück                                                                                                                                            |



<details>

<summary>An diesem Artikel beteiligt</summary>

* Lohoff44
* 50U7R34P3R

</details>
