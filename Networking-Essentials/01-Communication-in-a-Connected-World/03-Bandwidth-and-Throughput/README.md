# Bandwidth and Throughput

## Overview

Covers how the speed of data transfer on a network is described: **bandwidth** (the theoretical capacity of a medium) versus **throughput** (what is actually achieved), the units used to measure them, and why real-world throughput is almost always lower than the advertised bandwidth.

## Learning Objectives

- Define bandwidth and recognize its units of measure
- Define throughput and explain why it differs from bandwidth
- Explain how the slowest link limits end-to-end throughput

## Bandwidth

**Bandwidth** is the capacity of a medium to carry data — the amount of data that can (theoretically) flow from one place to another in a given amount of time. It is typically measured in the number of bits that can be sent across the media in one second.

Different physical media support the transfer of bits at different speeds. Physical media properties, current technologies, and the laws of physics all play a role in determining available bandwidth. High-bandwidth applications (streaming video, multiplayer gaming) need networks able to transmit and receive bits at a very high rate.

| Unit of Bandwidth | Abbreviation | Equivalence |
|---|---|---|
| Bits per second | bps | 1 bps = fundamental unit of bandwidth |
| Kilobits per second | Kbps | 1 Kbps = 1,000 bps = 10³ bps |
| Megabits per second | Mbps | 1 Mbps = 1,000,000 bps = 10⁶ bps |
| Gigabits per second | Gbps | 1 Gbps = 1,000,000,000 bps = 10⁹ bps |
| Terabits per second | Tbps | 1 Tbps = 1,000,000,000,000 bps = 10¹² bps |

## Throughput

**Throughput** is also the measure of bits transferred across the media over a given period of time — but it is the *actual* rate achieved, and it usually does **not** match the specified bandwidth.

Factors that influence throughput:

- The amount of data being sent and received over the connection
- The types of data being transmitted
- The **latency** created by the number of network devices between source and destination

**Latency** = the amount of time, including delays, for data to travel from one given point to another.

Throughput does not account for the validity or usefulness of the bits. Many messages on the network aren't destined for a user application at all (e.g. network control messages that regulate traffic and correct errors), but they still consume throughput.

### The slowest link rule

In a network with multiple segments, throughput can never be faster than the **slowest link** on the path from sender to receiver. Even if most segments are high-bandwidth, a single lower-bandwidth segment slows down the throughput of the whole path.

Online speed tests can be used to measure the throughput of an internet connection.

## Key Takeaways

- **Bandwidth = capacity (theoretical maximum); throughput = what you actually get.** Throughput is almost always lower.
- Bandwidth units scale by factors of 1,000: bps → Kbps → Mbps → Gbps → Tbps.
- Latency, traffic volume, data type, and non-user (control) traffic all pull throughput below the advertised bandwidth.
- End-to-end throughput is bounded by the slowest link in the path — one slow segment is the bottleneck for the entire connection.
