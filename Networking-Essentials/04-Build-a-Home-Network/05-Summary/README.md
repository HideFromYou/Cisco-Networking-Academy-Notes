# Build a Home Network — Summary

## Overview

End-of-module recap (4.5.1 "What Did I Learn in this Module?"). It restates the four topics of the module; the details live in their own sections.

## Recap

- **Home Network Basics** — Most home networks consist of at least two separate networks: the public network coming in from the service provider, and the home network behind the router, which is connected to the internet. The home router most likely has both wired and wireless capabilities. A home network is a small LAN whose devices usually connect to an integrated router and to each other to exchange information.
  - Wireless LAN technology is fairly easy and inexpensive to install. Advantages: mobility, scalability, flexibility, cost savings, reduced installation time, and reliability in harsh environments.
  - Besides the integrated router, many kinds of devices connect to a home network: desktop computers, gaming systems, smart TV systems, printers, scanners, security cameras, and climate control devices.
  - Small business and home routers typically have two primary types of ports: **Ethernet ports** and **internet ports**. Besides the wired ports, many home routers include a radio antenna and a built-in wireless access point.
- **Network Technologies in the Home** — Wireless technologies use **electromagnetic waves** to carry information between devices. The electromagnetic spectrum includes radio and television broadcast bands, visible light, x-rays, and gamma rays; some types of waves are not suitable for carrying data, and other parts of the spectrum are regulated by governments and licensed to organizations for specific applications.
  - Certain **unlicensed** sections of the spectrum are used in consumer products, including the Wi-Fi routers in most homes. The wireless technologies most used in home networks are in the unlicensed **2.4 GHz and 5 GHz** ranges.
  - **Bluetooth** uses the 2.4 GHz band. The modern wireless LAN technologies use 2.4 GHz and 5 GHz and conform to the various **IEEE 802.11** standards. Unlike Bluetooth, 802.11 devices transmit at a much higher power level, giving them greater range and improved throughput.
  - Some devices still benefit from a wired switch connection. The most commonly used wired protocol is **Ethernet**. Directly connected devices use an Ethernet patch cable, usually **unshielded twisted pair (UTP)**. **Category 5e** is the most common wiring in a LAN; the cable has 4 pairs of wires, twisted to reduce electrical interference. Homes without UTP wiring can use other technologies, such as **powerline**, to distribute wired connectivity.
- **Wireless Standards** — The **IEEE 802.11** standard governs the WLAN environment, using the 2.4 GHz and 5 GHz bands. Collectively these technologies are called **Wi-Fi**; the **Wi-Fi Alliance** tests wireless LAN devices from different manufacturers. Wireless routers using 802.11 have several settings to configure:
  - **Network mode** — the type of technology to support, e.g. 802.11b, 802.11g, 802.11n, or Mixed Mode.
  - **Network Name (SSID)** — identifies the WLAN; all devices that want to join must use the same SSID.
  - **Standard Channel** — the channel used for communication. By default it is set to **Auto**, so the access point picks the optimum channel.
  - **SSID Broadcast** — whether the SSID is broadcast to all devices in range. Enabled by default.
  - 802.11 can give more throughput depending on the environment. If all devices use the same 802.11 standard, maximum speeds for that standard are possible. If the access point accepts only one standard, devices that don't use it can't connect. A **mixed mode** environment can include devices using any of the existing Wi-Fi standards.
  - The SSID tells wireless devices (called **STAs**) which WLAN they belong to and which other devices they can communicate with. The SSID broadcast lets devices discover the network name automatically; when it is disabled, the SSID must be entered manually on each wireless device.
- **Set Up a Home Router** — Many home wireless routers have an **automatic setup utility** for the basic settings. To connect over a wired connection, plug an Ethernet patch cable into the computer's network port and the other end into a **LAN port** on the router.
  - Once the NIC link lights show a working connection, the computer needs an IP address. Most routers are set up so the computer gets one automatically from a local **DHCP server** configured on the router.
  - Before entering the configuration utility (or configuring through a web browser), decide how the network will be used: what to name it and which devices should connect. It is **not good practice to include the device model or brand name in the SSID**, since internet searches can expose security weaknesses.
  - Who can access the network depends on how you plan to use it. Many routers support **MAC address filtering** to specify exactly who is allowed on the wireless network: more secure, but less flexible when connecting new devices. Some routers support **guest access**, a special SSID coverage area that allows open access but restricts it to the internet only.
