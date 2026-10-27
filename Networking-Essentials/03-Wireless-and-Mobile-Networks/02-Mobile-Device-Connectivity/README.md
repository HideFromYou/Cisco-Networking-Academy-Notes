# Mobile Device Connectivity

## Overview

Covers how mobile devices connect over Wi-Fi, cellular data, and Bluetooth: the security precautions for Wi-Fi, how to join networks and toggle cellular data on Android and iOS, and how Bluetooth pairing works.

> The lesson also contains a video, 3.2.5 *Bluetooth Configuration on a Windows Laptop*, not included in the material.

## Learning Objectives

- Configure mobile devices for wireless connectivity

## Mobile Devices and Wi-Fi

Mobile devices let people send and receive voice, video, and data without being tied to a physical location (internet cafes, campus wireless networks for sign-ups, lectures, and assignments). As devices grow more powerful, tasks that needed large wired computers can now run on mobile devices over wireless networks.

Almost all mobile devices can connect to Wi-Fi, and it is advisable to when possible because:

- Data used over Wi-Fi does **not count against the cellular data plan**.
- Wi-Fi radios use **less power** than cellular radios, which conserves battery.

Security precautions for Wi-Fi on mobile devices:

- Never send login or password information in **plaintext** (unencrypted).
- Use a **VPN** when sending sensitive data, if possible.
- Enable security on home networks.
- Use **WPA2 or higher** encryption.

## Wi-Fi Settings

Android and Apple iOS are the two most popular mobile operating systems, and each has settings to connect to wireless networks.

**Connecting within range:** turn Wi-Fi on; the device searches for available networks and lists them. Touch a network and enter the password if needed.

**Moving between networks:**
- Out of range of one Wi-Fi network, the device tries another Wi-Fi network in range.
- If no Wi-Fi network is in range, it uses the **cellular data network**.
- With Wi-Fi on, it automatically joins any network it has connected to before. For a new network it either shows a list of available networks or asks whether to connect.

## Configure Mobile Wi-Fi Connectivity

If the device doesn't prompt to join a network, the network's **SSID broadcast** may be turned off or the device may not be set to connect automatically; configure it manually. SSIDs and passphrases must be typed **exactly** as entered on the wireless router, or the device won't connect (the router rejects a wrong key).

- **SSID** — the name assigned to a wireless network.
- **Passphrase** — what we normally call the "wireless password".

**Manual connection on Android:**
1. Settings > Add network
2. Enter the network SSID
3. Touch Security and select a security type
4. Touch Password and enter the password
5. Touch Save

**Manual connection on iOS:**
1. Settings > Wi-Fi > Other
2. Enter the network SSID
3. Touch Security and select a security type
4. Touch Other Network
5. Touch Password and enter the password
6. Touch Join

Mobile operating systems are updated often and customized by manufacturers, so the exact steps may differ; the manufacturer's website has manuals for each device.

## Configure Cellular Data Settings

Cellular data plans are offered by most carriers, but bandwidth limits and charges vary widely by carrier and by plan, so many users only use cellular data when Wi-Fi isn't available.

| OS | Turn cellular data on/off |
|---|---|
| **Android** | Settings > More (under Wireless and Networks) > Mobile Networks > Data enabled |
| **iOS** | Settings > Cellular Data > on/off |

Mobile devices are preprogrammed to use Wi-Fi if one is available and the device can connect to the access point and **receive an IP address**; otherwise they use cellular data if configured. Transitions are usually not obvious to the user: for example, moving from 4G to 3G coverage turns off the 4G radio and turns on the 3G radio **without losing the connection**.

## Simple Connectivity with Bluetooth

Cellular and Wi-Fi can be hard to configure and need extra equipment (towers, access points), and cables aren't always practical for headsets or speakers. **Bluetooth** is a simple alternative: wireless, automatic, and very low power, which saves battery. **Up to eight** Bluetooth devices can be connected at once.

Examples of Bluetooth use:

- **Hands-free headset** — earpiece with a microphone for calls
- **Keyboard or mouse** — easier input on a mobile device
- **Stereo control** — connect to a home or car stereo to play music
- **Car speakerphone** — speaker and microphone for calls
- **Tethering** — share a network connection with another mobile device or computer (also possible over Wi-Fi or a cable such as USB)
- **Mobile speaker** — portable speakers for high-quality audio without a stereo system

## Bluetooth Pairing

**Pairing** is when two Bluetooth devices establish a connection to share resources. Both radios are turned on and one device searches for others; the others must be in **discoverable (visible)** mode. A discoverable device transmits, on request:

- Name
- Bluetooth class
- Services the device can use
- Technical information, such as features or the Bluetooth specification it supports

A **PIN** (a number, numeric code, or passkey) may be requested to authenticate the pairing. It is stored by the pairing services, so it doesn't have to be entered again; a headset and phone then pair automatically when the headset is turned on in range.

**Pair with Android:**
1. Put the device in discoverable mode
2. Find the device's connection PIN
3. Settings > Wireless and networks
4. Touch Bluetooth to turn it on
5. Touch the Bluetooth tab
6. Touch Scan for devices
7. Touch the discovered device
8. Type the PIN
9. Touch the device name again to connect

**Pair with iOS:**
1. Put the device in discoverable mode
2. Find the device's connection PIN
3. Settings > Bluetooth
4. Touch Bluetooth to turn it on
5. Touch the discovered device
6. Type the PIN

Always check the manufacturer's documentation for your model, since the steps change with OS updates.

## Key Takeaways

- Prefer Wi-Fi when available: it saves cellular data and battery. Protect it with WPA2 or higher, a VPN for sensitive data, and never plaintext credentials.
- A device uses Wi-Fi first (if it can join and get an IP address), then cellular data; switching between networks, and between 4G and 3G, is seamless.
- SSID and passphrase must match the router exactly when joining manually.
- Bluetooth is for simple, low-power, short-range links (up to 8 devices); devices must be discoverable to pair, and a PIN may be needed once.
- Wi-Fi, cellular, and Bluetooth can all be in use at once, each with a different role.
