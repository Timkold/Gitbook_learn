# 🌟 Wie fange ich an?

**Agenten** sind ein Dienst zur Erfassung des Gerätestatus und zur Übertragung der Daten an das Überwachungssystem. Sie helfen dabei, die Leistung, Funktionalität und den Zustand der Infrastruktur zu überwachen, um Probleme frühzeitig zu erkennen.

### **🔗 Verbindung:**

Ein Agent verbindet sich mit Geräten über Protokolle (SSH, HTTP API, SNMP) und liest deren Status aus.

### **Agent in HashCare:**

* &#x20;Wird auf dem Server der Plattform installiert, auf der sich die Geräte befinden.
* Liest Metriken von Geräten im gleichen Netzwerk über IP-Adressen aus und überträgt sie an das Monitoring.

#### **Wie erstelle ich einen Agenten?**

1\. Gehe zum Menü **Agenten**.

2\. Klicke auf die Schaltfläche **Neuen Agenten erstellen**.

### **Status der Agenten:**

🟢 **Grün** – Der Agent ist aktiv.

🔴 **Rot** – Der Agent ist inaktiv.

🟡 **Gelb** – Es gibt sowohl aktive als auch inaktive Agenten.

<figure><img src="../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

## **Schritte zur Erstellung:**

1\. Klicke auf **Neuen Agenten erstellen**.

2\. Wähle im Feld **Modus** die Option **Intern**.

3\. Lade den Agenten über den Link herunter.

_Die Installationsanleitung kann über den Link geöffnet werden._

4\. Fülle das Feld **Name** aus (Pflichtfeld).

⚠️ Falls das Feld leer bleibt, ist die Schaltfläche **Erstellen** nicht aktiv.

<figure><img src="../.gitbook/assets/image (36).png" alt="" width="448"><figcaption></figcaption></figure>

## **🌐 Hinzufügen von Subnetzen:**

* Das Feld **Netzwerke** ist optional.
* Eingabeformat: `XX.XX.XX.XX/XX`
* `XX.XX.XX.XX` – IP-Adresse eines Geräts oder Subnetzes.
* &#x20;`/XX` – Subnetzmaske (zwischen 0 und 32).

Beispiel: `10.4.21.32/27`

* &#x20;**Netzwerkadresse**: `10.4.21.32`
* &#x20;**Hostbereich**: `10.4.21.33 – 10.4.21.62`
* &#x20;**Broadcast**: `10.4.21.63`

### **➕ So fügst du Subnetze hinzu:**

* Klicke auf **Hinzufügen**, um bis zu 5 Felder hinzuzufügen.
* **Limit**: maximal 125.000 IP-Adressen in Subnetzen.

## **⚙️ Installation des Agenten:**

1\. Führe folgenden Befehl aus:  
`<Pfad zur Datei>/hashcare-agent -Dapi-key=<Schlüssel>`

<figure><img src="../.gitbook/assets/Снимок экрана 2025-01-13 в 15.17.22.png" alt=""><figcaption></figcaption></figure>

2\. **API-Schlüssel**: Kopiere ihn aus dem entsprechenden Feld.

## 🔍 Aktivierung des Agenten:

**Interner Agent** wird nach erfolgreichem Start auf dem Server aktiviert.

**Angezeigt werden:**

* **🖥️ Agenten-IP**
* **📜 Version**
* **📊 Anzahl der Geräte** (wird alle 1–5 Minuten aktualisiert).

— Geräte aus Subnetzen werden automatisch hinzugefügt und mit ihren Daten ausgefüllt.

Weitere Informationen zu den Funktionen findest du im Bereich „HashCare“.
