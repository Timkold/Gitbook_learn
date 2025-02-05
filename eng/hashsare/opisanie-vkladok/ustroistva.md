# Devices

To collect data with an external agent, it is necessary to create devices with specified parameters. Devices are linked to a rack; creation is not possible without a link. By default, no devices are present.

### Devices Table

• Search — enter characters to filter by asset tag.

• Data Center, Room, Rack — filters for selecting devices in specific zones.

• Add Device — button for creation.

### Table Fields

• Device ID — unique system number.

• Model — determined by the agent or set manually; firmware is specified.

• Hashrate — current performance (Th/s):

🟢 Green circle — hashrate is greater than 0.

🔴 Red circle — hashrate is 0 or undefined.

• Worker Name — pool and device name (determined by the agent or manually).

• IP Address — automatically determined or set manually.

• S/N — serial number, determined by the agent or manually.

• Location — DC / Room / Rack (links to objects).

• Edit — button for parameter settings.

<figure><img src="../../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.32.30.png" alt=""><figcaption></figcaption></figure>

## Creating a Device via Form

1\. Go to the **Devices** menu.

2\. Click the **Add New Device** button.

3\. In the opened window, enter the following data:

• **Device Type** — model (dropdown menu with search function). _Required._

• **Asset Tag** — unique device name in the Hashcare system. _Required._

• **Serial Number** — _Required._

• **IP Address** — must match the pattern: ^(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9])$. _Required._

• **MAC Address** — must match the pattern: ^\[a-fA-F0-9]:\[a-fA-F0-9]{2}{5}$.

• **Shelf Number** — free shelf number depending on the rack.

* Cannot be 0. _Error: “Must be greater than or equal to 1”._
* Cannot exceed the maximum number of shelves in the rack. _Error: “error.codes.rack\_exceed\_max\_size”._
* Must be a number. _Error: “Invalid format”._

• **Slot Number** — free slot number on the shelf.

* Cannot be 0. _Error: “Must be greater than or equal to 1”._
* Cannot exceed the maximum number of slots on the shelf.
* Must be a number. _Error: “Invalid format”._

• **Stratum Pool URLs** — up to 3 addresses. _Optional._

• **Worker Name** — device name on the pool. _Required._

• **Pool Name** — pool name. _Required._

• **Rack** — select from existing racks. _Required._

• **Firmware Type** — _Required._

4\. Click **Create**.

<figure><img src="../../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.32.50.png" alt="" width="375"><figcaption></figcaption></figure>

### Importing Devices via List <a href="#importing-devices-via-list" id="importing-devices-via-list"></a>

1. Go to the **Devices** menu.
2. Select the appropriate option from the dropdown menu.
3. Select a **.csv** file from the hard drive.
4. If successfully uploaded, a message will appear: **"File successfully uploaded"**.

<figure><img src="../../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.33.32.png" alt="" width="279"><figcaption></figcaption></figure>

**Example of a CSV Table**

<figure><img src="../../../.gitbook/assets/Снимок экрана 2024-12-19 в 23.34.15.png" alt=""><figcaption></figcaption></figure>

## **Editing a Device**

1\. Click the **three dots** button next to the required device.

2\. Select **Edit**.

_**Editable parameters:**_

• **Device Type** — model. A dropdown menu with a search function. _Required._

• **Asset Tag** — unique device name in Hashcare. _Required._

• **Serial Number** — _Required._

• **IP Address** — must match the pattern: ^(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9])$. _Required._

• **MAC Address** — must match the pattern: ^\[a-fA-F0-9]:\[a-fA-F0-9]{2}{5}$. _Required._

• **Shelf Number** — free shelf number.

* Cannot be 0. _Error: “Must be greater than or equal to 1.”_
* Cannot exceed the maximum number of shelves. _Error: “error.codes.rack\_exceed\_max\_size.”_
* Must be a number. _Error: “Invalid format.”_

• **Place Number** — free slot number on the shelf.

* Cannot be 0. _Error: “Must be greater than or equal to 1.”_
* Cannot exceed the maximum number of slots.
* Must be a number. _Required._

• **Pool Stratum URLs** — up to 3 addresses. _Optional._

• **Worker Name** — device name on the pool. _Required._

• **Pool Name** — pool name. _Required._

• **Rack** — select from existing racks. _Required._

• **Firmware Type** — _Required._

• **Change Shelf Count (Height)** — must be between 1 and 10.

• **Change Slot Count (Width)** — must be between 1 and 10.

• **Change Room** — reassign the rack to another room.

<figure><img src="../../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.34.09.png" alt="" width="375"><figcaption></figcaption></figure>

3\. Click **Update** to save changes.

## Editing Devices via CSV File <a href="#editing-devices-via-csv-file" id="editing-devices-via-csv-file"></a>

You can edit multiple devices using a CSV file. Upload a CSV file containing devices that are already in the system.

1. The main identifier is the **MAC address** — if the MAC in the CSV matches an existing device, other details will be updated accordingly.
2. If the MAC address is not found in Hashcare, a new device will be created with the CSV parameters.

## **Deleting a Device** <a href="#deleting-a-device" id="deleting-a-device"></a>

1. Click the **three dots** button next to the required device.
2. Select **Delete**.
3. In the confirmation window, click **Confirm**.

<figure><img src="../../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.35.08.png" alt="" width="375"><figcaption></figcaption></figure>

## Device Details:

• **Model**

Automatically determined by the internal agent or set manually. Includes factory hashrate.

• **IP Address**

Automatically determined by the internal agent or set manually.

• **Firmware**

Automatically detected or set manually.

• **Serial Number (S/N)**

Automatically detected or set manually.

## Power

• **Wattage**

A static value set for each device model.

* **W/TH -** A relative value calculated as the ratio of nominal consumption to the nominal hash rate of the model.

• **Nominal Hashrate**

The factory hash rate value obtained by the internal agent from the ASIC.

### Additional Information

• **Worker Name**

Consists of the pool name and the device name in the pool. It is determined automatically by the internal agent or set manually in the device settings.

• **MAC Address**

Automatically determined by the internal agent during device polling or set manually in the device settings.

<figure><img src="../../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.35.45.png" alt=""><figcaption></figcaption></figure>

### Metrics:

• **Estimated Revenue (PPS | FPPS):**

* **PPS (Pay Per Share):** Fixed payment per share.
* **FPPS (Full Pay Per Share):** Includes commission revenue, higher than PPS.

• **Pool Revenue:**

The actual revenue from the pool for the selected period.

_Pool setup: "Pool Settings" → Create Pool._

• **Electricity Costs:**

Based on device power consumption and the tariff:

_(Power Consumption (W) × 24) ÷ 1000 × Tariff_

• **Profit:**

_{FPPS revenue} - {Electricity costs}_

### Hashrate Chart

• **Asic Hashrate** — the current hash rate reported by the device.\
• **Nominal Hashrate** — the manufacturer-declared hash rate.

### Plate Hashrate

Displays the performance of individual boards in an ASIC miner.

• Each board is labeled, e.g., SM 0, SM 1, SM 2.\
• Helps detect malfunctions that reduce the overall hash rate.

### Device Temperature

• **Board (boards) and chip (chip, PCB) temperature:** Displays heating of individual device components.

• **Air temperature (in/out):**

* **In** — temperature of incoming cool air.
* **Out** — temperature of outgoing heated air.

### Fan Speed

Displays the cooling fan speed in revolutions per minute (RPM).

• **In** — fans at the air intake.\
• **Out** — fans at the air exhaust.

### Energy Consumption

• **Asic Power** — current power consumption reported by the device.\
• **Nominal Power** — manufacturer-declared power consumption.

<figure><img src="../../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.37.58.png" alt=""><figcaption></figcaption></figure>
