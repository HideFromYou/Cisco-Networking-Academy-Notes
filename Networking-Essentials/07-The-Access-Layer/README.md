# Module 7: The Access Layer

## Overview

**Module objective:** Explain how devices access the network and how Ethernet frames are used to deliver data over a local network.

The module introduces Ethernet communication, frame structure, encapsulation, and the operation of switches at the access layer. It explains how network devices use addressing information to exchange data over a local network.

## Lessons

| # | Topic | Objective | Status |
|---|-------|-----------|--------|
| 7.0 | Introduction | — | ✅ |
| 7.1 | Ethernet Frames and Encapsulation | Describe Ethernet frames and the encapsulation process | ✅ |
| 7.2 | Ethernet Switching | Explain how switches forward Ethernet frames | ✅ |
| 7.3 | The Access Layer Summary | — | ✅ |

## Key Takeaways

- Ethernet is commonly used in LANs. Devices connect to an Ethernet network through a Network Interface Card (NIC).
- Each Ethernet NIC has a MAC address associated with its network interface.
- An Ethernet frame contains a preamble, Start Frame Delimiter (SFD), destination MAC address, source MAC address, Length/Type field, payload, and Frame Check Sequence (FCS).
- The preamble helps the receiving NIC synchronize with the incoming signal; the SFD marks the beginning of the frame.
- The destination MAC address identifies the intended interface on the local link, while the source MAC address identifies the sending interface.
- The Length/Type field indicates the payload length in IEEE 802.3 frames or the encapsulated protocol type in Ethernet II frames.
- The payload carries data from upper layers. The FCS uses a cyclic redundancy check (CRC) to detect errors in the frame.
- Encapsulation places one protocol data unit inside another as data moves down the protocol stack. De-encapsulation reverses this process at the receiving device.
- A Layer 2 switch learns its MAC address table by examining the source MAC address of incoming frames and associating it with the ingress port.
- When the destination MAC address is known, the switch forwards the frame through the associated port. When the destination is unknown, it floods the frame out the other ports in the same VLAN, except the ingress port.
- Dynamic MAC address table entries age out after a period of inactivity; the exact timer depends on the switch and its configuration.
