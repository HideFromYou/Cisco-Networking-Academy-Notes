# Set Up a Home Router

## Overview

Covers the first-time setup of a home wireless router (the wired connection, getting an IP address) and the design considerations to think through before configuring it: SSID naming, supported 802.11 standards, and who may access the network.

> The pasted material skipped from 4.4.2 to the Packet Tracer activity (4.4.4); page 4.4.3 was not included. MAC address filtering is mentioned in the module summary but not in the pages that were pasted.

## Learning Objectives

- Configure wireless devices for secure communications

## First Time Setup

Many home wireless routers have an **automatic setup utility** for the basic settings. These usually require a PC or laptop connected to a **wired port** on the router. If no device with a wired connection is available, the wireless client software on the laptop or tablet may need to be configured first.

**Wired connection steps:**
1. Plug an Ethernet patch cable into the network port on the computer.
2. Plug the other end into a **LAN port** on the router. **Do not** plug it into the port labeled **"Internet"**, which connects to the DSL or cable modem.

Some home routers have a **built-in modem**; if so, check that the connection type matches your internet service:

| Connection | Modem terminal |
|---|---|
| **Cable** | Coaxial terminal that accepts a **BNC-type** connector |
| **DSL** | Port for a telephone-type cable, usually an **RJ-11** connector |

Once the computer is connected and the **link lights on the NIC** show a working connection, it needs an **IP address**. Most routers are set up so the computer gets one automatically from a local **DHCP server** configured on the router. If it doesn't, check the router documentation and configure the PC or tablet with a **unique IP address, subnet mask, default gateway, and DNS** information.

## Design Considerations

Before entering the configuration utility (or configuring the router manually in a web browser), consider how the network will be used, so the configuration neither limits what you can do nor leaves the network unprotected.

- **SSID naming:** with SSID broadcast on, the name is visible to every wireless client within range, and it often gives away too much information. It is **not good practice to include the device model or brand name** in the SSID: default settings and known security weaknesses of wireless devices are easy to find on the internet.
- **Supported standards:** a device's radio works in a specific frequency range. A device that only has an 802.11 b/g radio will not connect if the router or AP accepts only 802.11n or 802.11ac. If all devices support the same standard, the network works at its optimum speed. If some devices don't support n or ac, enable **legacy mode**, which varies between router models but can combine 802.11a, b, g, n, and ac so legacy devices can connect. Some routers label legacy mode as **mixed mode**.
- **Who can access the network:** decide based on how you plan to use it. Some routers support **guest access**, a special SSID coverage area that allows open access but restricts it to **internet use only**.

## Packet Tracer Activity: Configure a Wireless Router and Client

The activity (4.4.4) has three parts: **Part 1 — Connect the Devices**, **Part 2 — Configure the Wireless Router**, **Part 3 — Configure IP Addressing and Test Connectivity**. Only the objectives were included in the material.

## Key Takeaways

- Connect to the router's **LAN** port (never the Internet port) for first-time setup; the computer normally gets its address from the router's built-in DHCP server.
- Cable modems use a coaxial terminal (BNC-type connector); DSL uses an RJ-11 telephone-type port.
- Don't put the device model or brand in the SSID.
- Legacy (mixed) mode lets older devices connect when the router would otherwise accept only newer standards.
- Guest access gives visitors internet-only access on a separate SSID.
