# Racks

A rack is an entity linked to a specific room, containing a set number of slots for devices. It displays data only for devices within it.

• You can create an unlimited number of racks in one room.

• By default, one rack is created and linked to the newly created room.

## "Racks" Table

• Search — search by name.

• Data center — select racks in a specific data center.

• Rooms — select racks within a room.

• Add new rack — button for creation.

## Table fields:

• ID — identifier in the database.

• Name — rack name.

• Data center — name of the data center.

• Room — the room to which the rack is linked.

• Editing — configure parameters.

<figure><img src="../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.08.20.png" alt=""><figcaption></figcaption></figure>

## Creating a Rack

1\. Go to the "Racks" menu.

2\. Click the "Create New Rack" button.

3\. In the pop-up window:

• Enter a name in the "Name" field.

• Specify the number of shelves (Height) from 1 to 10.

• Specify the number of slots per shelf (Width) from 1 to 10.

• Select a room from the dropdown list.

4\. Click the "Create" button.

<figure><img src="../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.08.39.png" alt="" width="375"><figcaption></figcaption></figure>

## Editing a Rack

1\. Click the _three-dot_ button next to the desired rack.

2\. Select "Edit"

3\. Make changes:

* New name.
* Number of shelves (Height) from 1 to 10.
* Number of slots per shelf (Width) from 1 to 10.
* Room to which the rack will be linked.

4\. Click "Update"

<figure><img src="../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.09.05.png" alt="" width="375"><figcaption></figcaption></figure>

## **Deleting a Rack:** <a href="#udalenie-data-centra" id="udalenie-data-centra"></a>

1. Click the three-dot button next to the desired rack.
2. Select "Delete" from the menu.
3. In the pop-up window, click "Confirm"

<figure><img src="../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.09.15.png" alt="" width="375"><figcaption></figcaption></figure>

## Navigating to the Rack Page

* In the "Racks" menu, click on the **Name** of the desired rack.

## Rack Page Contents

### **Details:**

• Size: width × height (e.g., 10×10).

• Place Count: total count (width × height).

• Devices Count:

* Total — inactive + online.
* Online — devices actively sending data.

<figure><img src="../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.10.09.png" alt=""><figcaption></figcaption></figure>

### Charts:

**• Hashrate:**

* Asic Hashrate — reported by the device.
* Nominal Hashrate — specified by the manufacturer.

**• Energy consumption:**

* Asic Power — reported by the device.
* Nominal Power — specified by the manufacturer.

**• Devices:**

* Active Asic — working devices.
* Total Asic — all devices, including inactive ones.

<figure><img src="../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.10.15.png" alt=""><figcaption></figcaption></figure>

### Rack Map

Displays a 2D layout with the specified number of slots and placed devices.

• Each slot displays:

* Actual hashrate.
* Maximum chip temperature.

• Display features:

* If hashrate or temperature = 0 or exceeds the normal range, the text turns red.
* To view current issues, switch the displayed characteristic in the top right corner.

<figure><img src="../../.gitbook/assets/Снимок экрана 2025-01-13 в 20.10.57.png" alt="" width="375"><figcaption></figcaption></figure>

### List of Devices on the Rack

\
Lists devices linked to the rack.

• The table includes:

* Device ID — unique identifier assigned by the system.
* Model — detected by the agent or set manually; displays firmware.
* Hashrate — current device performance:

🟢 Hashrate > 0

🔴 Hashrate = 0 or undefined

* Worker name — consists of the pool name and device, detected by the agent or set manually.
* IP address — automatically detected by the agent or set manually.

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>
