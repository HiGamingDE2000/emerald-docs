# TeamSpeak Server

Um deine Domain auf einen Minecraft Server weiterzuleiten, klicke in deiner Domain auf "**DNS Einstellungen**".

Sollte der TeamSpeak auf dem gleichen Account wie die Domain sein, so kannst du unter "Typ" **PRODUKT** auswählen, der Weiterleitung einen Namen geben und unter "Ziel" den passenden TeamSpeak Server wählen.

<figure><img src="../../.gitbook/assets/Ts-Produkt.png" alt=""><figcaption><p>TeamSpeak bei EmeraldHost</p></figcaption></figure>

Hostest du deinen TeamSpeak Server selbst oder bei einem anderen Hosting, so musst du folgende Einträge erstellen.&#x20;

## A-Eintrag

Wähle unter "Typ" den **A-Eintrag** aus.

Vergebe der Weiterleitung einen Namen woran du die TeamSpeak-Weiterleitung erkennen kannst.

Das "Ziel" ist die IP-Adresse deines TeamSpeak-Servers ohne Port.

<figure><img src="../../.gitbook/assets/A-Eintrag-TS (1).png" alt=""><figcaption><p>A Eintrag</p></figcaption></figure>

## SRV-Eintrag

Wähle unter "Typ" den **SRV-Eintrag** aus.

Klicke nun auf das leere Feld unter "Name".&#x20;

Trage nun folgende Daten in das geöffnete Fenster ein:

* Service Name -> \_ts3
* Protokoll -> UDP
* Name -> Kann leer gelassen werden außer du willst mit z.B. "ts." vor deiner Domain connecten

Bestätige die Eingaben nun mit "Speichern".

<figure><img src="../../.gitbook/assets/SRV-01.png" alt=""><figcaption><p>SRV Eintrag "Name"</p></figcaption></figure>

Klicke nun auf das leere Feld unter "Ziel".&#x20;

Trage nun folgende Daten in das geöffnete Fenster ein:

* Priorität -> 0
* Gewicht -> 5
* Port -> Der Port deines TeamSpeak-Servers
* Ziel -> Deine Domain | Solltest du unter "Name" eben etwas angegeben haben, so muss dies mit einem "." davor

Bestätige nun deine Eingaben mit "Speichern".

<figure><img src="../../.gitbook/assets/SRV-02.png" alt=""><figcaption><p>SRV Eintrag "Ziel"</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/SRV-03.png" alt=""><figcaption><p>SRV Eintrag erstellen</p></figcaption></figure>
