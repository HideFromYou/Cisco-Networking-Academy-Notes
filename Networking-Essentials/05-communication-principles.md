# Module 05 – Communication Principles

## 5.0 Introduction

Protocols are the rules that govern communication. Network devices use protocols to format, transmit, and interpret messages so that communication can take place reliably between different systems.

## 5.1 Communication Protocols

Human communication follows agreed rules. These include:

- An identified sender and receiver.
- An agreed method of communication.
- A common language and grammar.
- Appropriate speed and timing.
- Confirmation or acknowledgment that a message was received.

Network protocols follow the same general principles. They define how devices identify each other, format messages, control timing, and respond to received information.

**Protocol:** A set of rules that determines how devices communicate.
*(A set of rules that determines how devices communicate.)*

## 5.2 Communication Standards

Standards ensure that devices and software from different manufacturers can implement the same communication rules and interoperate.

**RFC (Request for Comments):** Documents used to describe, develop, and evolve Internet technologies and protocols.
*(Documents used to describe, develop, and evolve Internet technologies and protocols.)*

The **IETF (Internet Engineering Task Force)** develops and publishes Internet standards and related technical documents.

Organizations involved in networking standards and coordination include:

- **IEEE (Institute of Electrical and Electronics Engineers):** Develops standards used in networking technologies, including Ethernet and Wi-Fi.
- **IETF:** Develops Internet protocols and standards.
- **IANA (Internet Assigned Numbers Authority):** Coordinates global Internet numbering resources and protocol parameters.
- **ICANN (Internet Corporation for Assigned Names and Numbers):** Coordinates the Domain Name System and the global system of unique Internet identifiers.
- **ITU (International Telecommunication Union):** Develops international telecommunications standards.
- **TIA (Telecommunications Industry Association):** Develops standards for telecommunications and related infrastructure.

## 5.3 Network Communication Models

A protocol stack is a group of protocols that work together to provide network communication. Each protocol has a specific role.

Examples:

- **Ethernet:** Provides communication across a local network link between network interfaces.
- **IP (Internet Protocol):** Provides logical addressing and delivery from a source host toward a destination host across networks.
- **TCP (Transmission Control Protocol):** Provides reliable, ordered delivery of data.
- **HTTP (Hypertext Transfer Protocol):** Defines communication for transferring web resources, including HTML documents.

### TCP/IP and OSI Models

The TCP/IP model describes network communication in four layers. The OSI model describes it in seven layers.

| TCP/IP Model | Corresponding OSI Layers |
|---|---|
| Application | Application, Presentation, Session (Layers 7–5) |
| Transport | Transport (Layer 4) |
| Internet | Network (Layer 3) |
| Network Access | Data Link and Physical (Layers 2–1) |

The models provide complementary ways to describe how protocols cooperate during communication.

## Key Takeaways

- Protocols define the rules for formatting, transmitting, and interpreting messages.
- Communication requires agreed rules for sender, receiver, method, language, timing, and acknowledgment.
- Standards allow devices from different manufacturers to communicate.
- RFCs document Internet protocol development and evolution; the IETF develops Internet standards.
- Ethernet, IP, TCP, and HTTP perform different functions in the protocol stack.
- The TCP/IP model has four layers and the OSI model has seven, with corresponding layer mappings.
