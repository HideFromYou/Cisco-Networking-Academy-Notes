# Wireless Standards

## Overview

Covers the standards behind Wi-Fi (IEEE 802.11 and the Wi-Fi Alliance) and the basic settings of a wireless router: network mode, SSID, channel, and SSID broadcast.

## Learning Objectives

- Describe Wi-Fi

## Wi-Fi Networks

Standards exist so that wireless devices can communicate. They specify the RF spectrum used, data rates, how information is transmitted, and more.

- **IEEE** (Institute of Electrical and Electronics Engineers) is the main organization that creates wireless technical standards.
- The **IEEE 802.11** standard governs the **WLAN** environment. Amendments to 802.11 describe the characteristics of the different wireless standards. WLAN standards use the **2.4 GHz and 5 GHz** bands, and collectively these technologies are called **Wi-Fi**.
- The **Wi-Fi Alliance** tests wireless LAN devices from different manufacturers. The **Wi-Fi logo** on a device means the equipment meets the standards and should operate with other devices using the same standard.
- Standards keep improving connectivity and speed, and manufacturers implement new ones quickly in new products, so it is important to be aware of them as they appear.

## Wireless Settings

A wireless router using 802.11 has several settings to configure (Packet Tracer's *Basic Wireless Settings* interface shows them):

| Setting | Description |
|---|---|
| **Network Mode** | Determines the type of technology that must be supported, e.g. 802.11b, 802.11g, 802.11n, or Mixed Mode. |
| **Network Name (SSID)** | Identifies the WLAN. All devices that want to join must have the same SSID. |
| **Standard Channel** | The channel over which communication occurs. Set to **Auto** by default so the access point (AP) picks the optimum channel. |
| **SSID Broadcast** | Whether the SSID is broadcast to all devices in range. **Enabled** by default. |

SSID stands for **Service Set Identifier**.

### Network Mode

- 802.11 can provide increased throughput depending on the wireless environment. If all devices connect with the **same** 802.11 standard, **maximum speeds** for that standard are possible.
- If the AP is configured to accept only **one** 802.11 standard, devices that don't use it **cannot connect**.
- **Mixed mode** allows devices using any of the existing Wi-Fi standards, giving easy access to **older devices** that don't support the latest standards.

### SSID

- The wireless components must connect to the appropriate WLAN, and that is done with the SSID.
- The SSID is a **case-sensitive, alphanumeric string of up to 32 characters**, sent in the **header of all frames** transmitted over the WLAN.
- It tells wireless devices, called **wireless stations (STAs)**, which WLAN they belong to and which other devices they can communicate with. It is essentially the **name of the network**.

### SSID Broadcast

- Wireless routers broadcast their configured SSID by default, so clients can discover the network name automatically.
- When the broadcast is disabled, the SSID must be entered manually on each wireless device.
- Disabling the broadcast can make it harder for **legitimate** clients to find the network, but **turning it off is not enough** to stop unauthorized clients from connecting. All wireless networks should use the **strongest available encryption** to restrict unauthorized access.

## Key Takeaways

- IEEE 802.11 defines the WLAN standards on the 2.4 GHz and 5 GHz bands (Wi-Fi); the Wi-Fi Alliance certifies interoperability, shown by the Wi-Fi logo.
- Four basic router settings: network mode, SSID, channel (Auto by default), and SSID broadcast (enabled by default).
- A router limited to one 802.11 standard rejects devices that don't use it; mixed mode accepts older and newer devices.
- Hiding the SSID is not a security measure on its own; use the strongest available encryption.
