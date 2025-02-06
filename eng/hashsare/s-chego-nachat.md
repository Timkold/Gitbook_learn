# 🌟 Getting Started

An **agent** is a service for collecting device status data and transmitting it to the monitoring system. It helps track performance, operability, and infrastructure status for timely issue detection.

### 🔗 **Connection:**

The agent connects to devices via protocols (SSH, HTTP API, SNMP) and reads their status.

## 🔍 Agent in HashCare:

* Installed on the server at the site where the devices are located.
* Reads metrics from devices within the same network via IP addresses and transmits them to monitoring.

**How to Create an Agent:**

1. Go to the **Agent** menu.
2. Click the **Create New Agent** button.

## Agent Statuses:

🟢 **Green** — the agent is active.\
🔴 **Red** — the agent is inactive.\
🟡 **Yellow** — both active and inactive agents are present.

<figure><img src="../.gitbook/assets/Снимок экрана 2025-01-13 в 15.15.40.png" alt="" width="230"><figcaption></figcaption></figure>

## 🚀 Steps to Create an Agent:

1. Click the **Create New Agent** button.
2. In the **Mode** field, select **Internal**.
3. Download the agent from the link.

_Installation instructions can be accessed via the link._

4. Fill in the **Name** field (mandatory).

⚠️ If the field is empty, the **Create** button will be inactive.

<figure><img src="../.gitbook/assets/Снимок экрана 2025-01-13 в 15.17.00.png" alt="" width="375"><figcaption></figcaption></figure>

## 🌐 Adding Subnets:

• The **Networks** field is optional.\
• Input format: `XX.XX.XX.XX/XX`\
• `XX.XX.XX.XX` — IP address of a device or subnet.\
• `/XX` — subnet mask (from 0 to 32).

**Example:** `10.4.21.32/27`

* **Network Address:** `10.4.21.32`
* **Host Range:** `10.4.21.33 – 10.4.21.62`
* **Broadcast:** `10.4.21.63`

### ➕ **To Add Subnets:**

• Click **Add** to add up to 5 fields.\
• **Limit:** A maximum of 125,000 IP addresses in subnets.

## ⚙️ Installing the Agent:

1. Run the command: \<file\_path>/hashcare-agent -Dapi-key=\<key>

<figure><img src="../.gitbook/assets/Снимок экрана 2025-01-13 в 15.17.22.png" alt=""><figcaption></figcaption></figure>

2. **API Key:** Copy it from the corresponding field.

## 🔍 Agent Activation:

The **internal agent** activates after successfully launching on the server.

**The following information is displayed:**

* 🖥️ **Agent IP**
* 📜 **Version**
* 📊 **Number of devices** (updated every 1–5 minutes).

— Devices from subnets are automatically added with their data filled in.

You can explore the **personal account functionality** in the **"Hashcare"** section.
