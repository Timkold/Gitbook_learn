# Geräte

Damit ein externer Agent Daten sammeln kann, müssen Geräte mit den angegebenen Parametern erstellt werden. Geräte werden einem Rack zugewiesen – eine Erstellung ohne Zuordnung ist nicht möglich. Standardmäßig sind keine Geräte vorhanden.

### **Tabelle „Geräte“**

• Suchen – Eingabe von Zeichen zur Filterung nach Asset-Tag.

• Rechenzentrum, Raum, Rack – Filter zur Auswahl von Geräten in bestimmten Bereichen.

• Neues Gerät erstellen – Schaltfläche zur Erstellung.

### **Tabellenspalten**

• Geräte-ID – eindeutige Nummer im System.

• Modell – wird vom Agenten erkannt oder manuell festgelegt; zeigt die Firmware-Version an.

• Hashrate – aktuelle Leistung (TH/s):

🟢 Grüner Kreis – Hashrate größer als 0.

🔴 Roter Kreis – Hashrate gleich 0 oder nicht erkannt.

• Worker-Name – Pool- und Gerätename (wird vom Agenten erkannt oder manuell festgelegt).

• IP-Adresse – wird automatisch erkannt oder manuell festgelegt.

• S/N – Seriennummer, wird vom Agenten erkannt oder manuell festgelegt.

• Standort – Rechenzentrum / Raum / Rack (Verknüpfungen zu den Objekten).

• Bearbeiten – Schaltfläche zur Konfiguration der Parameter.

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

## **Erstellen eines Geräts über das Formular**

1\. Zum Menüpunkt **Geräte** wechseln.

2\. Auf die Schaltfläche **Neues Gerät erstellen** klicken.

3\. Im geöffneten Fenster die folgenden Daten eingeben:

• **Gerätetyp** – Modell (Dropdown-Menü mit Suchfunktion). _Pflichtfeld._

• **Asset-Tag** – eindeutiger Gerätename im Hashcare-System. _Pflichtfeld._

• **Seriennummer** – _Pflichtfeld._

• **IP-Adresse** – muss dem folgenden Muster entsprechen:\
^(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9])$. _Pflichtfeld._

• **MAC-Adresse** – muss dem folgenden Muster entsprechen:\
^\[a-fA-F0-9]:\[a-fA-F0-9]{2}{5}$.

• **Regalnummer** – Nummer eines freien Regals innerhalb des Racks.

* Darf nicht 0 sein. _Fehler: „Muss größer oder gleich 1 sein“._
* Darf die maximale Anzahl an Regalen im Rack nicht überschreiten. _Fehler: „error.codes.rack\_exceed\_max\_size“._
* Muss eine Zahl sein. _Fehler: „Ungültiges Format“._

• **Platznummer** – Nummer eines freien Platzes auf dem Regal.

* Darf nicht 0 sein. _Fehler: „Muss größer oder gleich 1 sein“._
* Darf die maximale Anzahl an Plätzen auf dem Regal nicht überschreiten.
* Muss eine Zahl sein. _Fehler: „Ungültiges Format“._

• **Pool-Stratum-URLs** – bis zu 3 Adressen. _Optional._

• **Pool-Worker-Name** – Gerätename im Pool. _Pflichtfeld._

• **Pool-Name** – Name des Pools. _Pflichtfeld._

• **Rack** – Auswahl aus bestehenden Racks. _Pflichtfeld._

• **Firmware-Typ** – _Pflichtfeld._

4\. Auf **Erstellen** klicken.

<figure><img src="../../.gitbook/assets/image (1) (1).png" alt="" width="448"><figcaption></figcaption></figure>

## **Importieren von Geräten per Liste** <a href="#importirovanie-ustrojstv-spiskom" id="importirovanie-ustrojstv-spiskom"></a>

1. Zum Menüpunkt **Geräte** wechseln.
2. In der Dropdown-Liste die Option **Geräte importieren (.csv)** auswählen.
3. Eine **.csv**-Datei von der Festplatte auswählen.
4. Nach erfolgreichem Upload erscheint die Meldung „Datei erfolgreich hochgeladen“.

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

**Beispiel einer CSV-Tabelle**

<figure><img src="../../.gitbook/assets/Снимок экрана 2024-12-19 в 23.34.15.png" alt=""><figcaption></figcaption></figure>

## **Gerät bearbeiten**

1\. Auf die Schaltfläche (drei Punkte) neben dem gewünschten Gerät klicken.

2\. Die Option **Bearbeiten** auswählen.

_**Verfügbare Parameter zur Änderung:**_

• **Gerätetyp** – Modell. Das Feld funktioniert als Dropdown-Menü mit einer Suchfunktion. _Pflichtfeld._

• **Asset-Tag** – eindeutiger Gerätename im Hashcare-System. _Pflichtfeld._

• **Seriennummer** – _Pflichtfeld._

• **IP-Adresse** – muss folgendem Muster entsprechen:\
^(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9])$.\
&#xNAN;_&#x50;flichtfeld._

• **MAC-Adresse** – muss folgendem Muster entsprechen:\
^\[a-fA-F0-9]:\[a-fA-F0-9]{2}{5}$.\
&#xNAN;_&#x50;flichtfeld._

• **Regalnummer** – Nummer eines freien Regals innerhalb des gewählten Racks.

* Darf nicht 0 sein. _Fehler: „Muss größer oder gleich 1 sein.“_
* Darf die maximale Anzahl an Regalen im Rack nicht überschreiten. _Fehler: „error.codes.rack\_exceed\_max\_size.“_
* Muss eine Zahl sein. _Fehler: „Ungültiges Format.“_

• **Platznummer** – Nummer eines freien Platzes im Regal.

* Darf nicht 0 sein. _Fehler: „Muss größer oder gleich 1 sein.“_
* Darf die maximale Anzahl an Plätzen im angegebenen Regal nicht überschreiten. _Fehler: „Ungültiges Format.“_
* Muss eine Zahl sein. _Pflichtfeld._

• **Pool-Stratum-URLs** – Stratum-Adressen. Es können 1 bis 3 Adressen hinzugefügt werden. _Optional._

• **Pool-Worker-Name** – Gerätename im Pool. _Pflichtfeld._

• **Pool-Name** – Name des Pools. _Pflichtfeld._

• **Rack** – Auswahl aus bestehenden Racks. _Pflichtfeld._

• **Firmware-Typ** – _Pflichtfeld._

• **Anzahl der Regale ändern** (Höhe) – muss größer oder gleich 1 und kleiner oder gleich 10 sein.

• **Anzahl der Plätze pro Regal ändern** (Breite) – muss größer oder gleich 1 und kleiner oder gleich 10 sein.

• **Raum ändern**, dem das Rack zugeordnet wird.

<figure><img src="../../.gitbook/assets/image (3).png" alt="" width="446"><figcaption></figcaption></figure>

3\. Auf **Aktualisieren** klicken, um die Änderungen zu speichern.

## **Bearbeiten von Geräten über eine CSV-Datei** <a href="#redaktirovanie-ustrojstv-cherez-csv-fajl" id="redaktirovanie-ustrojstv-cherez-csv-fajl"></a>

Es besteht die Möglichkeit, mehrere Geräte gleichzeitig über eine CSV-Datei zu bearbeiten. Dazu muss eine CSV-Datei mit einer Liste der bereits erstellten Geräte hochgeladen werden.

1. Das Hauptidentifikationsmerkmal ist die **MAC-Adresse** – wenn die MAC-Adresse eines bestehenden Geräts mit der MAC-Adresse in der CSV-Datei übereinstimmt, werden die übrigen Daten gemäß den Informationen in der CSV-Datei geändert.
2. Falls die MAC-Adresse nicht im Hashcare-System existiert, wird ein neues Gerät mit den in der CSV-Datei angegebenen Parametern erstellt.

## **Gerät löschen:**

1. Auf die Schaltfläche (_drei Punkte_) neben dem gewünschten Gerät klicken.
2. Die Option **Löschen** auswählen.
3. Im geöffneten Fenster auf die Schaltfläche **Bestätigen** klicken.

<figure><img src="../../.gitbook/assets/image (4).png" alt="" width="344"><figcaption></figcaption></figure>

## **Gerätedetails:**

• **Modell**

Wird automatisch vom internen Agenten erkannt oder manuell in den Geräteeinstellungen festgelegt. Enthält die werkseitige Hashrate.

• **IP-Adresse**

Wird automatisch vom internen Agenten beim Netzwerk-Scan erkannt oder manuell in den Geräteeinstellungen festgelegt.

• **Firmware**

Wird automatisch vom internen Agenten beim Gerät-Scan erkannt oder manuell in den Geräteeinstellungen festgelegt.

• **Seriennummer (S/N)**

Wird automatisch vom internen Agenten beim Gerät-Scan erkannt oder manuell in den Geräteeinstellungen festgelegt.

### **Leistung**

• **Nominale Leistung**

Ein statischer Wert, der für jedes Gerätemodell festgelegt ist.

* W/TH – eine relative Größe, die als Verhältnis des nominalen Verbrauchs zur nominalen Hashrate des Modells berechnet wird.

• **Nominale Hashrate**

Der werkseitige Hashrate-Wert, den der interne Agent aus dem ASIC ausliest.

### **Zusätzliche Informationen**

• **Worker-Name**

Besteht aus dem Namen des Pools und dem Namen des Geräts im Pool. Wird automatisch vom internen Agenten erkannt oder manuell in den Geräteeinstellungen festgelegt.

• **MAC-Adresse**

Wird automatisch vom internen Agenten beim Gerät-Scan erkannt oder manuell in den Geräteeinstellungen festgelegt.

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

### **Kennzahlen:**

**• Geschätzter Ertrag (PPS | FPPS):**

* PPS (Pay Per Share): Feste Zahlung pro Share.
* FPPS (Full Pay Per Share): Enthält Gebühreneinnahmen, höher als PPS.

**• Pool-Einnahmen:**

Der tatsächliche Ertrag aus dem Pool für den gewählten Zeitraum.

_Einstellung des Pools: „Pool-Einstellungen“ → Pool erstellen._

**• Stromkosten:**

Basieren auf der Leistung des Geräts und dem Tarif:\\

(Verbrauchte Leistung (W) × 24) ÷ 1000 × Tarif\\

**• Gewinn:**

{FPPS-Einnahmen} - {Stromkosten}

### **Hashrate-Diagramm**

• **Asic Hashrate** – aktuelle Hashrate, die vom Gerät gesendet wird.

• **Nominal Hashrate** – die vom Hersteller angegebene Hashrate.

### **Platten-Hashrate-Diagramm**

Zeigt die Leistung einzelner Platinen des ASIC-Miners.

• Jede Platine wird beispielsweise als SM 0, SM 1, SM 2 bezeichnet.

• Hilft, Fehler zu erkennen, die die Gesamt-Hashrate verringern.

### **Gerätetemperatur**

• Temperatur der Platinen (Boards) und Chips (Chip, PCB): Zeigt die Erwärmung einzelner Komponenten des Geräts.

• Lufttemperatur (Ein/Aus):

* **In** – Temperatur der einströmenden kalten Luft.
* **Out** – Temperatur der ausströmenden erwärmten Luft.

### **Lüftergeschwindigkeitsdiagramm**

Zeigt die Drehzahl der Kühlventilatoren in Umdrehungen pro Minute (RPM).

* **In** – Lüfter am Einlass des Luftstroms.
* **Out** – Lüfter am Auslass.

### **Energieverbrauchsdiagramm**

* **Asic Power** – aktueller Verbrauch, der vom Gerät gesendet wird.
* **Nominal Power** – vom Hersteller angegebener Verbrauch.

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>
