# Module 08 – The Internet Protocol

## 8.0 Introduction

IPv4 provides logical addressing for devices on a network. Every IPv4 packet contains a source IPv4 address and a destination IPv4 address.

## 8.1 IPv4 Addresses

An IPv4 address is a logical address assigned to a network interface.

- IPv4 addresses are 32 bits long.
- They are divided into four 8-bit octets.
- Each octet is represented as a decimal number from 0 to 255.
- The four octets are written in dotted-decimal notation (for example, `192.168.5.11`).

**IPv4 Address:** A logical address used to identify a network interface at the Internet Layer.
*(A logical address used to identify a network interface at the Internet Layer.)*

## 8.2 IPv4 Address Structure

An IPv4 address contains two parts:

- **Network portion:** Identifies the network.
- **Host portion:** Identifies an interface within that network.

A subnet mask identifies which bits belong to the network portion and which belong to the host portion.

Example:

- IPv4 address: `192.168.5.11`
- Subnet mask: `255.255.255.0`
- Network: `192.168.5.0`
- Host portion: `.11`

The prefix length `/24` means that the first 24 bits identify the network and the remaining 8 bits identify the host portion. It does **not** mean that the network supports only 24 devices.

For a conventional `/24` subnet:

- Total addresses: `2^8 = 256`
- Network address: `192.168.5.0`
- Broadcast address: `192.168.5.255`
- Traditionally usable host addresses: 254

Hierarchical addressing allows routers to forward packets toward networks instead of needing a separate route for every host.

## 8.3 Connectivity Test – Packet Tracer

In the Packet Tracer activity, a ping was sent to the web server at `172.33.100.50`. Three replies were received and one packet was lost. An initial timeout can occur while devices are starting or while address resolution is taking place.

**Ping:** Uses ICMP Echo Request and Echo Reply messages to test IP reachability.
*(Uses ICMP Echo Request and Echo Reply messages to test IP reachability.)*

Opening the same IP address in a browser tests a different service:

1. The client establishes a TCP connection with the server.
2. The client sends an HTTP request (for example, an HTTP GET).
3. The server returns an HTTP response containing the requested resource.

Ping tests IP reachability; browsing tests application-layer communication as well.

## Key Takeaways

- IPv4 addresses are 32-bit logical addresses written as four decimal octets.
- A subnet mask separates the network and host portions of an address.
- A prefix such as `/24` counts network bits; it is not a device count.
- Routers use hierarchical network addressing to forward packets between networks.
- ICMP ping tests reachability, while HTTP browsing tests access to a web service over TCP.
