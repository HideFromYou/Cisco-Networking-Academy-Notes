# Module 09 – IPv4 and Network Segmentation

## 9.0 Introduction

IPv4 addresses can be used for different communication types: unicast, broadcast, and multicast. IPv4 addresses are also categorized as public, private, or reserved/special-purpose. Network segmentation divides a network into smaller logical networks.

## 9.1 IPv4 Address Types

### Unicast

**Unicast:** One-to-one communication between a source and a destination.
*(One-to-one communication between a source and a destination.)*

A unicast packet is intended for one destination interface. The source IPv4 address of an ordinary packet is unicast. The destination may be unicast, broadcast, or multicast.

For example, when a user sends a message through a social-media service, the user's device communicates with the service's server using unicast. The server may then send a separate unicast communication to the recipient's device. The application-level recipient is not necessarily the immediate IP destination.

### Broadcast

**Broadcast:** One-to-all communication within a broadcast domain.
*(One-to-all communication within a broadcast domain.)*

A broadcast is addressed to all devices in the relevant broadcast domain.

- Limited broadcast: `255.255.255.255`
- Directed broadcast example for `172.16.4.0/24`: `172.16.4.255`

Routers do not forward ordinary IPv4 broadcasts between interfaces by default. IPv6 does not use broadcast; it uses multicast for comparable functions.

### Multicast

**Multicast:** One-to-selected-group communication.
*(One-to-selected-group communication.)*

IPv4 multicast addresses are in the range `224.0.0.0` through `239.255.255.255`. Devices that have joined the relevant multicast group process the traffic. OSPF uses the multicast address `224.0.0.5` for AllSPF routers.

## 9.2 Public and Private IPv4 Addresses

### Private IPv4 Address Ranges

RFC 1918 defines three private IPv4 address blocks:

| Private range | Address block |
|---|---|
| 10.0.0.0/8 | 10.0.0.0 – 10.255.255.255 |
| 172.16.0.0/12 | 172.16.0.0 – 172.31.255.255 |
| 192.168.0.0/16 | 192.168.0.0 – 192.168.255.255 |

Not every address beginning with `172` is private. Only the range from `172.16.0.0` through `172.31.255.255` belongs to the RFC 1918 private block.

**Private IPv4 Address:** An address intended for use within private networks and not routed globally on the public Internet.
*(An address intended for use within private networks and not routed globally on the public Internet.)*

**Public IPv4 Address:** A globally unique address that can be routed on the public Internet.
*(A globally unique address that can be routed on the public Internet.)*

### NAT and PAT

**NAT (Network Address Translation):** Translates IP addresses, commonly translating private internal addresses to a public address at the network edge.
*(Translates IP addresses, commonly translating private internal addresses to a public address at the network edge.)*

**PAT (Port Address Translation):** Allows multiple internal devices to share one public IPv4 address by tracking transport-layer port numbers.
*(Allows multiple internal devices to share one public IPv4 address by tracking transport-layer port numbers.)*

### Special IPv4 Addresses

- **Loopback – `127.0.0.0/8`:** Used by a host to send traffic to itself. `127.0.0.1` is the commonly used loopback address. A ping to it tests the local TCP/IP stack, not Internet connectivity.
- **Link-local/APIPA – `169.254.0.0/16`:** A host may self-assign an address in this range when it cannot obtain an address through normal configuration methods such as DHCP. It can support local communication in limited circumstances.

### Legacy Classful Addressing

Historically, IPv4 addresses were divided into classes:

| Class | Historical range / purpose |
|---|---|
| A | 0.0.0.0 – 127.255.255.255 |
| B | 128.0.0.0 – 191.255.255.255 |
| C | 192.0.0.0 – 223.255.255.255 |
| D | 224.0.0.0 – 239.255.255.255 (multicast) |
| E | 240.0.0.0 – 255.255.255.255 (experimental/reserved) |

Class A, B, and C historically used fixed network prefixes of /8, /16, and /24 respectively. Classful addressing has been replaced by classless addressing (CIDR). These historical ranges include reserved and special-purpose addresses; they should not be interpreted as entirely usable host ranges.

### IANA and Regional Internet Registries

IANA coordinates global IP address allocation and delegates address blocks to five Regional Internet Registries (RIRs):

- **AFRINIC:** Africa
- **APNIC:** Asia-Pacific
- **ARIN:** North America
- **LACNIC:** Latin America and parts of the Caribbean
- **RIPE NCC:** Europe, the Middle East, and Central Asia

Greece is served by RIPE NCC.

## 9.3 Network Segmentation

**Network Segmentation:** Divides a larger network into smaller logical networks (subnets).
*(Divides a larger network into smaller logical networks (subnets).)*

### Broadcast Domains

An Ethernet LAN uses broadcasts for tasks such as ARP address resolution. A Layer 2 switch forwards a broadcast out its other ports, except the port on which it arrived. A router does not forward Layer 2 broadcasts between its interfaces. Each router interface therefore separates broadcast domains.

DHCP clients initially use a DHCP Discover broadcast to locate a DHCP server. The DHCP process is commonly described as DORA:

1. Discover
2. Offer
3. Request
4. Acknowledgment (ACK)

The initial Discover is broadcast; the later messages are not necessarily all broadcasts.

### Why Segment a Network?

A large broadcast domain can generate substantial broadcast traffic. Devices must process broadcasts even when the traffic is not intended for a particular application.

Subnetting divides the network into smaller broadcast domains. For example, a large `172.16.0.0/16` network could be divided into smaller `/24` networks such as:

- `172.16.0.0/24`
- `172.16.1.0/24`

Broadcast traffic remains within its subnet. A router provides communication between the subnets when permitted.

Benefits of segmentation include:

- Reducing unnecessary broadcast traffic and improving performance.
- Applying security policies to control communication between subnets.
- Limiting the impact of excessive or abnormal broadcast traffic caused by misconfiguration, faulty devices, software issues, or malicious activity.

### Common Segmentation Approaches

- **By Location:** Separate networks for different floors, buildings, or sites.
- **By Group or Function:** Separate networks for departments such as Administration, HR, and Accounting.
- **By Device Type:** Separate networks for device categories such as computers, printers, and servers.

## Key Takeaways

- Unicast is one-to-one, broadcast is one-to-all within a broadcast domain, and multicast is one-to-selected-group.
- RFC 1918 defines the three private IPv4 address blocks: 10/8, 172.16/12, and 192.168/16.
- NAT translates addresses; PAT allows multiple internal devices to share a public address using port numbers.
- Loopback tests the local host's TCP/IP stack; link-local/APIPA addresses may be self-assigned when normal address configuration fails.
- IANA coordinates global IP address allocation through the five RIRs.
- Routers separate broadcast domains; switches forward Layer 2 broadcasts within the local broadcast domain.
- Subnetting reduces broadcast-domain size and can support performance and security policies.
