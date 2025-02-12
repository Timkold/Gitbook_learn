# Racks

Ein Rack ist eine Einheit, die einem bestimmten Raum zugeordnet ist und eine bestimmte Anzahl von Plätzen für Geräte enthält. Es zeigt nur die Daten der darin befindlichen Geräte an.

• In einem Raum kann eine unbegrenzte Anzahl von Racks erstellt werden.

• Standardmäßig wird ein Rack erstellt, das dem erstellten Raum zugeordnet ist.

## **Tabelle „Racks“**

• Suchen – Suche nach Namen.

• Rechenzentrum – Auswahl der Racks in einem bestimmten Rechenzentrum.

• Raum – Auswahl der Racks in einem bestimmten Raum.

• Neues Rack erstellen – Schaltfläche zur Erstellung.

## Tabellenspalten:

• ID – Identifikator in der Datenbank.

• Name – Name des Racks.

• Rechenzentrum – Name des Rechenzentrums.

• Raum – Der Raum, dem das Rack zugeordnet ist.

• Bearbeiten – Konfiguration der Parameter.

<figure><img src="../../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

## **Erstellen eines Racks**

1\. Zum Menü **Racks** wechseln.

2\. Auf die Schaltfläche **Neues Rack erstellen** klicken.

3\. Im geöffneten Fenster:

* Den Namen in das Feld **Name** eingeben.
* Anzahl der Ebenen (Höhe) von 1 bis 10 festlegen.
* Anzahl der Plätze pro Ebene (Breite) von 1 bis 10 festlegen.
* Einen Raum aus der Dropdown-Liste auswählen.

4\. Auf die Schaltfläche **Erstellen** klicken.

<figure><img src="../../.gitbook/assets/image (27).png" alt="" width="344"><figcaption></figcaption></figure>

## **Bearbeiten eines Racks**

1\. Auf die Schaltfläche _drei Punkte_ neben dem gewünschten Rack klicken.

2\. Die Option **Bearbeiten** auswählen.

3\. Änderungen vornehmen:

* Neuer Name.
* Anzahl der Ebenen (Höhe) von 1 bis 10.
* Anzahl der Plätze pro Ebene (Breite) von 1 bis 10.
* Der Raum, dem das Rack zugeordnet wird.

4\. Auf **Aktualisieren** klicken.

<figure><img src="../../.gitbook/assets/image (28).png" alt="" width="342"><figcaption></figcaption></figure>

## **Löschen eines Racks** <a href="#udalenie-data-centra" id="udalenie-data-centra"></a>

1. Auf die Schaltfläche _drei Punkte_ neben dem gewünschten Rack klicken.
2. Die Option **Löschen** auswählen.
3. Im geöffneten Fenster auf die Schaltfläche **Bestätigen** klicken.

<figure><img src="../../.gitbook/assets/image (30).png" alt="" width="343"><figcaption></figcaption></figure>

## **Navigation zur Rack-Seite**

* Im Menü **Racks** auf den **Namen** des gewünschten Racks klicken.

## **Inhalt der Rack-Seite**

### **Details:**

• Größe: Breite × Höhe (z. B. 10×10).

• Anzahl der Plätze: Gesamtzahl (Breite × Höhe).

• Anzahl der Geräte:

* Gesamt – inaktive + Online-Geräte.
* Online – Geräte, die Daten übertragen.

<figure><img src="../../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

### **Diagramme:**

**• Hashrate:**

* Asic Hashrate – vom Gerät übermittelt.
* Nominal Hashrate – vom Hersteller angegebene Leistung.

**• Energieverbrauch:**

* Asic Power – vom Gerät übermittelter Verbrauch.
* Nominal Power – vom Hersteller angegebener Verbrauch.

**• Geräte:**

* Active Asic – aktive Geräte.
* Total Asic – alle Geräte, einschließlich nicht funktionierender.

<figure><img src="../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

### **Rack-Karte**

Zeigt ein 2D-Schema mit der angegebenen Anzahl von Plätzen und den platzierten Geräten.

• Jede Zelle enthält:

* Aktuelle Hashrate.
* Maximale Chip-Temperatur.

• Besondere Anzeigeeigenschaften:

* Wenn die Hashrate oder Temperatur = 0 ist oder die Norm überschreitet, wird die Schrift rot.
* Zum Anzeigen aktueller Probleme kann die dargestellte Eigenschaft in der oberen rechten Ecke umgeschaltet werden.

<figure><img src="../../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

### **Geräteliste im Rack**

Zeigt eine Liste der dem Rack zugewiesenen Geräte.

• Die Tabelle enthält:

* Geräte-ID – eindeutige Kennung, die vom System zugewiesen wird.
* Modell – vom Agenten erkannt oder manuell festgelegt; zeigt die Firmware-Version.
* Hashrate – aktueller Wert des Geräts:

&#x20;     🟢 Hashrate > 0

&#x20;     🔴 Hashrate = 0 oder nicht erkannt

* Worker-Name – besteht aus dem Pool-Namen und dem Gerätenamen, wird vom Agenten bestimmt oder manuell festgelegt.
* IP-Adresse – wird automatisch vom Agenten erkannt oder manuell festgelegt.

<figure><img src="../../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>
