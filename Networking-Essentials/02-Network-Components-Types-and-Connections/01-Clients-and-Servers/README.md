# Clients and Servers

## Overview

Covers the roles hosts play on a network: servers that provide information and services, clients that request and display it, peer-to-peer networks where one machine does both, and how a single host can hold multiple roles at once.

## Learning Objectives

- Explain the roles of clients and servers in a network
- Describe peer-to-peer networks and applications, with their advantages and disadvantages
- Explain how one host can run several server and client roles

## Client and Server Roles

A **host** is any computer connected to a network that participates directly in network communication; hosts can send and receive messages. In modern networks a host can act as a **client**, a **server**, or **both** — the **software installed** on the computer determines which role it plays.

| Role | What it is | Example |
|---|---|---|
| **Server** | Host with server software that provides information/services (email, web pages) to other hosts | Web server software, file server software, email server software |
| **Client** | Host with client software that requests and displays information obtained from a server | A web browser (Chrome, Edge, Safari, Firefox), an email client |

- **Each service needs its own server software** — e.g. a host needs web server software to provide web services.
- Every online destination is provided by a server somewhere on a network connected to the global internet.

## Peer-to-Peer (P2P) Networks

Client and server software usually run on separate computers, but one computer can run both at once. In small businesses and homes, many computers act as both servers and clients — this is a **peer-to-peer (P2P) network**.

- The simplest P2P network = two directly connected computers (wired or wireless), each acting as client or server as needed.
- Larger P2P networks need a network device, such as a **switch**, to interconnect the computers.
- Larger businesses usually need **dedicated servers** because of the volume of service requests.

| Advantages | Disadvantages |
|---|---|
| Easy to set up | No centralized administration |
| Less complex | Not as secure |
| Lower cost — network devices and dedicated servers may not be required | Not scalable |
| Fine for simple tasks such as transferring files and sharing printers | Devices acting as both client and server can slow their performance |

## Peer-to-Peer Applications

A **P2P application** lets a device act as both client and server within the same communication: every client is a server and every server is a client. Each end device must provide a user interface and run a background service. Instant messaging is the example — both sides can send and receive at the same time.

Some P2P applications use a **hybrid** system: resource sharing is decentralized, but the **indexes** pointing to resource locations are kept in a centralized directory. Each peer asks an index server where a resource lives on another peer.

## Multiple Roles in the Network

- One computer with server software can serve **one or many clients** simultaneously.
- One computer can run **multiple types of server software** (a home/small-business machine can be file server, web server, and email server at once).
- One computer can run **multiple types of client software** — one client per required service — so a host can connect to several servers at the same time (checking email, browsing, instant messaging, and listening to internet radio together).

## Check Your Understanding

1. *Computer with software to provide information such as email or web pages to other devices is a:* → **server**
2. *A smartphone uses a web browser to request and display a web page — it is a:* → **client**
3. *Two computers communicating as both client and server form a:* → **peer-to-peer network**

## Key Takeaways

- Client/server is about **software roles**, not hardware: the installed software decides whether a host acts as client, server, or both.
- Every service needs its own server software and its own matching client software.
- P2P trades simplicity and low cost for security, scalability, and central management — which is why larger networks use dedicated servers.
- A single host can hold many roles at once, which is how one machine can serve files, web pages, and email while also browsing and messaging.
