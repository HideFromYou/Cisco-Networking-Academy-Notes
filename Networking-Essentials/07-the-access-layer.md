# Module 07 – The Access Layer

## 7.0 Introduction

The Access Layer is the edge of a network where end devices connect. It is a hierarchical network design concept, not a layer of the OSI model.

The TCP/IP Network Access layer broadly corresponds to the OSI Physical and Data Link layers.

## 7.1 Ethernet Frames

Ethernet carries data across a local network link using frames. An Ethernet frame contains the following fields:

| Field | Purpose |
|---|---|
| Preamble | Helps the receiving network interface synchronize with the incoming frame. |
| Start Frame Delimiter (SFD) | Indicates the beginning of the frame. |
| Destination MAC Address | Identifies the intended destination on the local link. |
| Source MAC Address | Identifies the sending network interface. |
| Length/Type | Indicates the payload length or the encapsulated protocol type, depending on the Ethernet format. |
| Data/Payload | Carries the encapsulated data, such as an IP packet. |
| Frame Check Sequence (FCS) | Uses a CRC value to detect errors in the frame. |

**MAC Address:** Identifies a network interface at the Data Link Layer.
*(Identifies a network interface at the Data Link Layer.)*

The FCS allows the receiver to detect whether a frame was corrupted during transmission. It is for error detection, not error correction.

## 7.2 Encapsulation and De-encapsulation

As data moves down the protocol stack at the sender, each layer adds its own information. This process is called **encapsulation**.

At the receiver, the corresponding headers and trailers are processed and removed as the data moves up the stack. This is called **de-encapsulation**.

An Ethernet payload can contain an IP packet, which in turn carries transport-layer and application data.

## 7.3 IPv6 Header Overview

The IPv6 header has a fixed length of 40 bytes and includes these fields:

| Field | Purpose |
|---|---|
| Version | Identifies the IP version (6). |
| Traffic Class | Used for traffic priority and handling. |
| Flow Label | Identifies packets belonging to a particular flow. |
| Payload Length | Indicates the length of the data following the IPv6 header. |
| Next Header | Identifies the type of header that follows, such as an extension header or an upper-layer protocol. |
| Hop Limit | Limits how many routers a packet can pass through. |
| Source Address | IPv6 address of the sender. |
| Destination Address | IPv6 address of the destination. |

## 7.4 Ethernet Switching and MAC Address Tables

A Layer 2 switch uses a MAC address table to decide where to forward Ethernet frames.

- The switch learns a source MAC address and associates it with the port on which the frame arrived.
- If the destination MAC address is known, the switch forwards the frame through the associated port.
- If the destination is an unknown unicast address, the switch floods the frame out the other ports in the relevant VLAN, except the incoming port.
- Dynamically learned MAC table entries age out after a period of inactivity. The exact aging time depends on the switch configuration; a commonly shown example is around five minutes.

A switch learns from the **source** MAC address, not the destination MAC address.

## 7.5 Frame Delivery at the Network Interface

For ordinary unicast traffic, a network interface generally processes frames addressed to its MAC address and discards frames addressed to other unicast destinations. Broadcast and relevant multicast frames are exceptions. A network interface in promiscuous mode can also capture frames not normally addressed to it.

## Key Takeaways

- The Access Layer is where end devices connect; it is not an OSI layer.
- Ethernet frames include synchronization fields, source and destination MAC addresses, a Length/Type field, payload, and FCS.
- FCS uses CRC for error detection.
- Encapsulation adds protocol information as data moves down the stack; de-encapsulation processes it at the receiver.
- The IPv6 base header is fixed at 40 bytes and includes eight main fields.
- A Layer 2 switch learns source MAC addresses and incoming ports to build its MAC address table.
- Unknown unicast frames are flooded within the relevant VLAN, except through the incoming port.
