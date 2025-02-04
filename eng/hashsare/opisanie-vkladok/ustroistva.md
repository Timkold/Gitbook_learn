# Devices

To collect data with an external agent, it is necessary to create devices with specified parameters. Devices are linked to a rack; creation is not possible without a link. By default, no devices are present.

\
Devices Table
------------------



• Search — enter characters to filter by asset tag.

• Data Center, Room, Rack — filters for selecting devices in specific zones.

• Add Device — button for creation.



## Table Fields



• Device ID — unique system number.

• Model — determined by the agent or set manually; firmware is specified.

• Hashrate — current performance (Th/s):

• 🟢 Green circle — hashrate is greater than 0.

• 🔴 Red circle — hashrate is 0 or undefined.

• Worker Name — pool and device name (determined by the agent or manually).

• IP Address — automatically determined or set manually.

• SN — serial number, determined by the agent or manually.

• Location — DC / Room / Rack (links to objects).

• Edit — button for parameter settings.

<figure><img src="../../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.32.30.png" alt=""><figcaption></figcaption></figure>

## Creating a Device via Form

1\. Go to the **Devices** menu.

2\. Click the **Add New Device** button.

3\. In the opened window, enter the following data:

\
• **Device Type** — model (dropdown menu with search function). _Required._

• **Asset Tag** — unique device name in the Hashcare system. _Required._

• **Serial Number** — _Required._

• **IP Address** — must match the pattern: ^(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9])$. _Required._

• **MAC Address** — must match the pattern: ^\[a-fA-F0-9]:\[a-fA-F0-9]{2}{5}$.

• **Shelf Number** — free shelf number depending on the rack.

• Cannot be 0. _Error: “Must be greater than or equal to 1”._

• Cannot exceed the maximum number of shelves in the rack. _Error: “error.codes.rack\_exceed\_max\_size”._

• Must be a number. _Error: “Invalid format”._

• **Slot Number** — free slot number on the shelf.

• Cannot be 0. _Error: “Must be greater than or equal to 1”._

• Cannot exceed the maximum number of slots on the shelf.

• Must be a number. _Error: “Invalid format”._

• **Stratum Pool URLs** — up to 3 addresses. _Optional._

• **Worker Name** — device name on the pool. _Required._

• **Pool Name** — pool name. _Required._

• **Rack** — select from existing racks. _Required._

• **Firmware Type** — _Required._

\
4\. Click **Create**.
-------------------

<figure><img src="../../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.32.50.png" alt="" width="375"><figcaption></figcaption></figure>



## Importing Devices via List <a href="#importing-devices-via-list" id="importing-devices-via-list"></a>

1. Go to the **Devices** menu.
2. Select the appropriate option from the dropdown menu.

<figure><img src="../../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.33.32.png" alt="" width="279"><figcaption></figcaption></figure>

1. Select a **.csv** file from the hard drive.
2. If successfully uploaded, a message will appear: **"File successfully uploaded"**.

**Example of a CSV Table**

<figure><img src="../../../.gitbook/assets/Снимок экрана 2024-12-19 в 23.34.15.png" alt=""><figcaption></figcaption></figure>

**Editing a Device**

\


1\. Click the **three dots** button next to the required device.

2\. Select **Edit**.

\
Editable parameters:

• **Device Type** — model. A dropdown menu with a search function. _Required._

• **Asset Tag** — unique device name in Hashcare. _Required._

• **Serial Number** — _Required._

• **IP Address** — must match the pattern: ^(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9])$. _Required._

• **MAC Address** — must match the pattern: ^\[a-fA-F0-9]:\[a-fA-F0-9]{2}{5}$. _Required._

• **Shelf Number** — free shelf number.

• Cannot be 0. _Error: “Must be greater than or equal to 1.”_

• Cannot exceed the maximum number of shelves. _Error: “error.codes.rack\_exceed\_max\_size.”_

• Must be a number. _Error: “Invalid format.”_

• **Slot Number** — free slot number on the shelf.

• Cannot be 0. _Error: “Must be greater than or equal to 1.”_

• Cannot exceed the maximum number of slots.

• Must be a number. _Required._

• **Stratum Pool URLs** — up to 3 addresses. _Optional._

• **Worker Name** — device name on the pool. _Required._

• **Pool Name** — pool name. _Required._

• **Rack** — select from existing racks. _Required._

• **Firmware Type** — _Required._

• **Change Shelf Count (Height)** — must be between 1 and 10.

• **Change Slot Count (Width)** — must be between 1 and 10.

• **Change Room** — reassign the rack to another room.

\


<figure><img src="../../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.34.09.png" alt="" width="375"><figcaption></figcaption></figure>

3\. Click **Update** to save changes.

## Editing Devices via CSV File <a href="#editing-devices-via-csv-file" id="editing-devices-via-csv-file"></a>

You can edit multiple devices using a CSV file. Upload a CSV file containing devices that are already in the system.

1. The main identifier is the **MAC address** — if the MAC in the CSV matches an existing device, other details will be updated accordingly.
2. If the MAC address is not found in Hashcare, a new device will be created with the CSV parameters.

### **Deleting a Device** <a href="#deleting-a-device" id="deleting-a-device"></a>

1. Click the **three dots** button next to the required device.
2. Select **Delete**.
3. In the confirmation window, click **Confirm**.

<figure><img src="../../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.35.08.png" alt="" width="375"><figcaption></figcaption></figure>

\
Device Details

\
• **Model**

Automatically determined by the internal agent or set manually. Includes factory hashrate.

• **IP Address**

Automatically determined by the internal agent or set manually.

• **Firmware**

Automatically detected or set manually.

• **Serial Number (S/N)**

Automatically detected or set manually.

\
**Power**

• **Nominal Power** — static value for each model.

• **W/TH** — power efficiency.

• **Nominal Hashrate** — factory hashrate.

\
**Additional Information**

• **Worker Name** — consists of pool name and device name.

• **MAC Address** — automatically detected or set manually.

\

<figure><img src="../../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.37.58.png" alt=""><figcaption></figcaption></figure>
