# 🧑🏭 Das Job-System

Ein neuer NPC ist aufgetaucht und hat ein neues Feature im Gepäck. Ihr könnt nun Aufträge vergeben, damit euch andere Spieler Items erfarmen. Hierbei stellt ihr einen Auftrag ein, welches Item für euch gefarmt werden soll und in welcher Menge.

Das Ganze funktioniert mindestens stackweise (oder in größeren Mengen) und es können nur ausgewählte Materialien gesucht werden. Andere Items lassen sich nicht beauftragen.

### Wie erstelle ich einen Auftrag?

Ich benötige einen bestimmten Materialblock – Wie erhalte ich diesen?

1. Job-Menü aufrufen
2. "Meine Aufträge" aufrufen
3. Neuen Auftrag anlegen
4. Auftragsdetails wählen
5. Informationen bestätigen
6. Auftrag freigeben

***

1. Das Job-System lässt sich über einen Job-NPC oder über den Befehl `/jobs`  aufrufen. Der Job-NPC ist in der Hauptstadt zu finden.

{% hint style="success" %}
**Tipp:** Am besten den gesuchten Materialblock bereits im Inventar dabei haben!
{% endhint %}

2. Es öffnet sich ein GUI mit allen eingestellten Aufträgen von Spielern. Mit dem Button „Meine Aufträge“ (Redstone – Komparator) gelangst du in deine Auftragsliste.

<figure><img src="https://lh7-us.googleusercontent.com/mw30eALsnM-_nuVxeMwT5rP71CtxZfEht3-GfSuQ07eseCa4xRrmSiFZq_PyV7F3Bx22XkjvRD0D6hCsnB5DKh0X67vUNhJMymW4tJ9zH91iOgKpPw9XnWAIthjuq_WH0y_XePfIQq5hLglp2k-mdoQ" alt=""><figcaption><p>Der Button "Meine Aufträge" öffnet eure Auftragsliste</p></figcaption></figure>

3. In diesem Fenster werden alle Aufträge, die du erstellt hast, angezeigt. \
   Hierüber hast du die Übersicht über deine bestehenden Aufträge und zusätzlich die Möglichkeit, einen neuen Auftrag zu erstellen (Grüner + Kopf Button) „Neuen Auftrag erstellen“.\
   Hinweis: Abholbereite Items werden mit einem Leucht-Effekt angezeigt.
4. Sobald du auf den (Grüner + Kopf Button) „Neuen Auftrag erstellen“ klickt, öffnet sich ein weiteres Fenster mit folgenden Buttons

{% tabs %}
{% tab title="Obere Reihe" %}
*   Barriere „Item wählen“

    Hier gibst du an, welches Material du sucht. Dafür musst du diesen Material-Block zumindest einmal im Inventar haben. Klicke in deinem Inventar auf den gesuchten Block; dieser wird automatisch hinterlegt.
*   Goldbarren „Preis pro Stack“

    Sobald du auf den Goldbarren klickst, musst du im Chat eingeben, wie viel du bereit bist, je Stack zu bezahlen.

{% hint style="success" %}
Tipp: Realistische Preise erhöhen eure Chance, dass andere Spieler diesen Block an Euch verkaufen.&#x20;
{% endhint %}

{% hint style="success" %}
Tipp: Eine Übersicht der Preise erhaltet Ihr auf Grieferwert.
{% endhint %}
{% endtab %}

{% tab title="Mittlere Reihe" %}
* 64x Barrieren „Anzahl 1x Stack“\
  Dies bedeutet, dass Ihr einen Stack des gesuchten Materials sucht bzw. kauft.
* Truhe „Anzahl 1x Kiste“\
  Dies bedeutet, dass Ihr 27x Stacks des gesuchten Materials sucht bzw. kauft.
* 2x Truhe „1x Doppelkiste“\
  Dies bedeutet, dass Ihr 54x Stacks des gesuchten Materials sucht bzw. kauft.
* Güterlore „Anzahl Stacks“\
  Dies bedeutet, dass Ihr individuell die Anzahl der Stacks des gesuchten Materials im Chat eingeben könnt.
{% endtab %}

{% tab title="Untere Reihe" %}
* Redstone "Abbrechen"\
  Mit diesem Button brecht ihr den aktuellen Auftrag ab und kehrt in eure Auftragliste zurück.\
  Der Button ist nicht verfügbar,. wenn ihr den Auftrag fertig gestellt habt.
* Barriere "Unvollständig"\
  Dieser Button zeigt an, das Informationen zum Erstellen des Auftrags fehlen.&#x20;
* Grüner Farbstoff "Auftrag erstellen"\
  Dieser Button ist erst verfügbar, wenn alle Informationen zum Auftrag eingegeben wurden. Er ersetzt die Barriere.
{% endtab %}
{% endtabs %}

<figure><img src="https://lh7-us.googleusercontent.com/L-FKo2l8rO-LhMY0ViOcPRkAse9KBb2L3VuJIx9T7I5RGqrNPpXR9sCE3CBQ9Lu7LOhX8Hm_rX_SDNUh5D_m21LejtmLCb3rQ0ctG0s66453f-lgimkfx2fRwdjBhFGU8FCy-FyrhTNbUeLPf-xJaY0" alt=""><figcaption><p>Die Erstellung eines Auftrags erfordert gewisse Informationen.</p></figcaption></figure>

5. Rechts unten erscheint ein grüner Farbstoff Button, sobald alle Informationen hinterlegt sind.

{% hint style="success" %}
Tipp: Wenn du über den Button fährst, werden dir die Kosten für den Auftrag zzgl. Gebühren angezeigt.
{% endhint %}

<figure><img src="https://lh7-us.googleusercontent.com/rnb9v7hfjFDTg9UR0KrT7EFeRcYeiZOJS6y1NLsS3A3zXNcflaUQ3ArtCjuPYjNh46ISv4tafEbbi1DBLpyT_wZU1rDia0xHPXWWMZVHlppeO0Bz95yIrsglQRQzt70_yCgHrVumclyfXj5TfheSylY" alt=""><figcaption><p>Der Mouseover des Buttons "Auftrag erstellen" gibt euch eine Übersicht eures Auftrags.</p></figcaption></figure>

6. Mit einem Klick auf den Button erstellst du deinen Auftrag. Denke daran, dass du dieses Geld direkt an den NPC bezahlen musst.

***

### Ich möchte einen Auftrag stornieren  - Wie geht das?

Möchtest du einen Auftrag stornieren, gehe wie folgt vor:

1. Rufe das Jobs-Menü über einen Jobs-NPC oder per Befehl `/jobs` auf.
2. Es öffnet sich das GUI mit allen eingestellten Aufträgen von Spielern. Mit dem Knopf (Redstone – Komparator) „Meine Aufträge“ gelangst du in deine Auftragliste.

<figure><img src="https://lh7-us.googleusercontent.com/OSs3B0vTdae9Yz7311wTk9OpQqMnKnEyLQD5wOnUuVNrFD8IIR4NAZa180buxXpVcU_Gmy14DgbQrqVtq_30z-4DafZEAclCxVsYegafB85aeMW8KVQZhogEh-Au4xIFeN6VuFR9wekZ9BA2PhiHswQ" alt=""><figcaption><p>Mit dem Button "Meine Aufträge" öffnest du deine persönliche Auftragsliste.</p></figcaption></figure>

3. Hier findest du eine Übersicht deiner Aufträge. Mit einem Rechtsklick auf den jeweiligen Auftrag kannst du diesen stornieren.&#x20;

<figure><img src="https://lh7-us.googleusercontent.com/0HTc3J928Xt_mmNrGoYkvPzs-Q5AWVo-9QqwiehHRqD_VNw-oGJKxmybGwUgaUJmEnRLtnEm8Mg1mXJau7AG1QAYEpAzVwKMp4yj6jZOI0VVPObz3gnT5pOM7jzctrCohCIatBXtf9TuSfOmgdgPhmU" alt=""><figcaption><p>Alle Aufträge, welche noch nicht erledigt sind, findest du hier. </p></figcaption></figure>

4. Job-Menü beim Jobs-NPC oder per Befehl `/jobs`  aufrufen, um dein Geld abzuholen. Es erscheint ein Goldbarren neben dem Knopf „Meine Aufträge“. Wenn du auf diesen klickst, erhältst du den verbleibenden Betrag zurück.

<figure><img src="https://lh7-us.googleusercontent.com/Skj1K0QIzn0Vwd7j7mRnc6xlLErgSF318b6rz9NY-zaNrO_kCegym13V6IY6zmjvP-y3H7r_C5kv8qwUiTQL1eL296FEY4zzySVh7EotXJ89HMbLNQS2ki6NUn2RAJ2CO8s0MsU7tOZNVp7yQITM3L0" alt=""><figcaption><p>Hast du Aufträge abgebrochen ist im Job-Menü ein neuer Button verfügbar, um dein Geld abzuholen.</p></figcaption></figure>



<details>

<summary>An diesem Artikel beteiligt</summary>

* Zheng\_Aokiji
* 50U7R34P3R

</details>
