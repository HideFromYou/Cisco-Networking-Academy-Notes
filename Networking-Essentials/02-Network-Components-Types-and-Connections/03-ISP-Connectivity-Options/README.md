# ISP Connectivity Options

## Overview

Covers what an Internet Service Provider (ISP) is, how ISPs form the backbone of the internet, how a home network connects to an ISP, and the common connection technologies (cable, DSL, fiber, cellular, satellite, dial-up).

## Learning Objectives

- Describe the role and services of an ISP
- Explain the difference between a direct modem connection and a router-based connection
- Compare cable and DSL connections
- Recognize additional connectivity options

## ISP Services

An **ISP** provides the link between a home network and the internet. It can be a local cable provider, a landline telephone provider, the cellular network behind a smartphone plan, or an independent provider that leases bandwidth on another company's physical infrastructure.

Many ISPs also sell extra services to subscribers: FTP hosting, application and media hosting, web hosting, equipment co-location, POP internet access, voice over IP, technical support, plus email accounts, network storage, automated backup, and security services.

**ISPs and the backbone**
- Each ISP connects to other ISPs, forming a network of links that interconnects users worldwide.
- ISPs are connected **hierarchically**, so traffic generally takes the shortest path from source to destination.
- The **internet backbone** is a set of high-speed data links connecting service-provider networks in major metropolitan areas worldwide. Its primary medium is **fiber-optic cable**, usually installed underground to connect cities within continents, and under the sea to connect continents, countries, and cities.

## ISP Connections

The backbone is a complex web of fiber with expensive switches and routers directing traffic between hosts; home users don't see any of it.

| Option | Description |
|---|---|
| **Single PC, direct modem connection** | The simplest option: a modem connects a computer straight to the ISP. **Not recommended** — the computer is unprotected on the internet. |
| **Router-based (integrated router)** | The most common option: a wireless integrated router connects to the ISP via a modem. The router includes a **switch** for wired hosts and a **wireless AP** for wireless hosts, and provides **client IP addressing** and **security** for inside hosts. |

## Cable and DSL

Most home users don't connect with fiber. The two most common methods:

| | Cable | DSL (Digital Subscriber Line) |
|---|---|---|
| Provided by | Cable television providers | Telephone service providers |
| Medium | Same coaxial cable that carries cable TV | Telephone line |
| Device | Cable modem separates the internet data signal from the other signals and provides an Ethernet connection | High-speed DSL modem separates the DSL signal from the telephone signal and provides an Ethernet connection |
| Characteristics | High bandwidth, always on | High bandwidth, always on |

**DSL channels:** the line is split into three — one for **voice** calls (so you can take calls without disconnecting from the internet), one **faster download** channel, and one **upload** channel (usually slightly slower than download). Quality and speed depend mainly on **phone line quality** and **distance from the telephone company's central office** — the farther away, the slower the connection.

## Additional Connectivity Options

Other options for home users: **cellular**, **satellite**, and **dial-up telephone**. The choice depends on geographical location and service-provider availability.

| Option | Description | Pros | Cons |
|---|---|---|---|
| **Cellular** | Uses the cell phone network; works wherever there is a signal. Performance is limited by the phone and the cell tower it connects to. | Real benefit in areas with no other connectivity, and for people constantly on the move | Carrier usually meters bandwidth and may charge extra beyond the data plan |
| **Satellite** | A satellite modem and dish at the user's side talk to a satellite, which relays to a dish and router at the satellite service provider. Path: laptop → satellite modem → dish → satellite → ISP's dish → ISP router. Good for homes/offices without DSL or cable. | Speeds generally good (vary by contract); available where nothing else is | Dish needs a clear line of sight (hard in heavily wooded areas or with overhead obstructions); equipment and installation costs can be high, then a moderate monthly fee |
| **Dial-up telephone** | Any phone line plus a modem; the user calls the ISP's access phone number. | Inexpensive; useful for mobile access while traveling | Low bandwidth, not enough for large transfers; consider only when faster options are unavailable |
| **Fiber to the premises** | In metropolitan areas, many apartments and small offices are connected directly with fiber-optic cable. | Higher bandwidth and more services (internet, phone, TV) | Depends on location |

The choice of connection varies with geographical location and service provider availability.

## Key Takeaways

- An ISP is the bridge between a local network and the internet; ISPs interconnect hierarchically over a fiber-optic backbone.
- A router (not a bare modem) is what securely connects a home network to the ISP — it combines switching, wireless access, IP addressing, and security.
- Cable rides the TV coaxial line; DSL rides the telephone line and degrades with distance from the central office.
- Availability decides the option: fiber, cable, DSL, cellular, satellite, or dial-up.
