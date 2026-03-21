<!-- markdownlint-disable-file -->
# Week 1 — The OSI Model

**Phase:** 1 — Foundations  
**Date:** 14 March 2026  
**Status:** ✅ Complete

---

## What is the OSI Model?

The OSI (Open Systems Interconnection) model is a framework that
describes how data travels from one device to another across a network.
It has 7 layers, each with a specific job.

---

## The 7 Layers

| Layer | Name | Unit | Device | Key Protocols |
|-------|------|------|--------|---------------|
| 7 | Application | Data | — | HTTP, HTTPS, FTP, DNS, SMTP |
| 6 | Presentation | Data | — | SSL, TLS, JPEG, MP3 |
| 5 | Session | Data | — | NetBIOS, PPTP |
| 4 | Transport | Segments | — | TCP, UDP |
| 3 | Network | Packets | Router | IP, ICMP, ARP |
| 2 | Data Link | Frames | Switch | Ethernet, ARP |
| 1 | Physical | Bits | Hub | — |

---

## Layer Summaries

**Layer 7 — Application**  
The interface between the user and the network. Where user-facing
applications like browsers and email clients operate.

**Layer 6 — Presentation**  
Translates, encrypts, and compresses data. SSL/TLS encryption happens
here. Handles formats like JPEG and MP3.

**Layer 5 — Session**  
Establishes, maintains, and terminates sessions between devices.
Handles synchronisation — allows interrupted transfers to resume.

**Layer 4 — Transport**  
Breaks data into segments. TCP guarantees delivery (accuracy).
UDP prioritises speed over accuracy. Uses port numbers.

**Layer 3 — Network**  
Handles IP addressing and routing. Routers operate here.
Data unit is called a Packet.

**Layer 2 — Data Link**  
Handles MAC addressing. Switches operate here.
Data unit is called a Frame.

**Layer 1 — Physical**  
Transmits raw bits (0s and 1s) over cables or wireless signals.
Hubs operate here — they broadcast to all devices (obsolete).

---

## Key Comparisons

**TCP vs UDP**
| TCP | UDP |
|-----|-----|
| Connection-oriented | Connectionless |
| Reliable — guarantees delivery | Fast — no guarantee |
| Used for: file downloads, web, email | Used for: video calls, streaming, gaming |

**Hub vs Switch**
| Hub | Switch |
|-----|--------|
| Layer 1 | Layer 2 |
| Broadcasts to all devices | Sends only to correct device |
| Causes collisions | No collisions between ports |
| Obsolete | Used in every modern LAN |

**IP Address vs MAC Address**
| IP Address | MAC Address |
|------------|-------------|
| Layer 3 — logical address | Layer 2 — physical address |
| Changes per network | Burned into hardware at factory |
| Used for routing | Used for local delivery |

---

## Memory Trick

**Top to bottom:**  
> "All People Seem To Need Data Processing"  
> Application → Presentation → Session → Transport → Network → Data Link → Physical

**Bottom to top:**  
> "Please Do Not Throw Sausage Pizza Away"  
> Physical → Data Link → Network → Transport → Session → Presentation → Application

---

## Resources Used
- Kurose & Ross — Chapter 1
- Odom CCNA Guide — Chapter 1
- Professor Messer — The OSI Model (YouTube)
- NetworkChuck — OSI Model (YouTube)