# Module 1 — Network Architecture

**Date:** September 3, 2026  
**Course:** Connect and Protect: Networks and Network Security

## What I Learned

Today I learned the fundamentals of computer networks, network components, cloud computing, IP and MAC addresses, and the TCP/IP model.

---

## 1. Network Fundamentals

A **network** is a group of connected devices.

Networks can vary in size:

- **LAN (Local Area Network)** — spans a small area such as a home, school, or office building.
- **WAN (Wide Area Network)** — spans a large geographic area such as a city, state, or country.

### Important Network Terms

- **Bandwidth** — The maximum data transmission capacity over a network, measured by bits per second.
- **Speed** — The rate at which a device sends and receives data, measured by bits per second.
- **Data packet** — A basic unit of information that travels from one device to another within a network.
- **Port** — A software-based location that organizes the sending and receiving of data between devices on a network.

---

## 2. Network Components and Devices

### Modem

A modem connects a router to the internet and brings internet access to the LAN.

### Router

A router connects multiple networks together and directs traffic between networks.

### Switch

A switch makes connections between specific devices on a network by sending and receiving data between them.

A switch uses a **MAC address table** to direct data packets to the correct device.

### Hub

A hub broadcasts information to every device on the network.

Because a hub broadcasts information to all connected devices, it can be vulnerable to eavesdropping.

### Firewall

A firewall is a security device that monitors incoming and outgoing traffic on a network.

---

## 3. Client-Server Model

In the client-server model:

- **Clients** send requests for information or services.
- **Servers** perform requests and provide information or services.

Examples of servers include:

- DNS servers
- File servers
- Corporate mail servers

Servers can also communicate with databases to provide information and services to clients.

---

## 4. Cloud Computing

**Cloud computing** is the practice of using remote servers, applications, and network services that are hosted on the internet instead of on local physical devices.

Cloud service providers can offer:

- On-demand storage
- Processing power
- Analytics

### Cloud Network

A **cloud network** is a collection of servers or computers that stores resources and data in remote data centers that can be accessed via the internet.

---

## 5. IP Addresses

An **Internet Protocol (IP) address** is a unique string of characters that identifies the location of a device on the internet.

### IPv4

IPv4 addresses are written as four 1–3 digit numbers separated by decimal points.

Example:

`172.16.254.1`

Each number can contain a value from **0–255**.

### Public IP Address

A public IP address is assigned by an internet service provider (ISP) and is connected to a geographic location.

Devices on a local network can share the same public-facing IP address through mechanisms such as network address translation (NAT) or a forwarding proxy.

---

## 6. MAC Addresses

A **Media Access Control (MAC) address** is a unique alphanumeric identifier assigned to each physical device on a network.

Switches use MAC address tables to determine where to direct data on a local network.

---

## 7. TCP/IP Model

The TCP/IP model is a framework used to visualize how data is organized and transmitted across a network.

The four layers are:

1. **Application Layer**
2. **Transport Layer**
3. **Internet Layer**
4. **Network Access Layer**

### Application Layer

Examples:

- HTTP
- TLS
- DNS

### Transport Layer

Examples:

- TCP
- UDP

### Internet Layer

The Internet layer uses:

- IP (IPv4 and IPv6)

### Network Access Layer

Examples:

- Ethernet
- Wireless LAN
- ARP

---

## 8. TCP and UDP

### TCP

**Transmission Control Protocol (TCP)** allows two devices to form a connection and stream data.

### UDP

**User Datagram Protocol (UDP)** is a connectionless protocol that does not establish a connection between devices before transmissions.

---

## 9. Protocol Number

The protocol number in an IP packet tells the receiving device what to do with the information in the packet.

Examples include:

- TCP
- UDP
- ICMP

---

## 10. Packet Sniffing

**Packet sniffing** is the practice of capturing and inspecting data packets across a network.

This can be useful for analyzing network communications and investigating network activity.

---

## Key Takeaways

- Networks are groups of connected devices.
- LANs cover smaller areas, while WANs cover larger geographic areas.
- Routers connect multiple networks.
- Switches connect specific devices and use MAC address tables to direct traffic.
- Hubs broadcast information to connected devices.
- Cloud computing uses remote servers, applications, and network services.
- IP addresses identify the location of devices on a network.
- MAC addresses identify physical devices on a network.
- The TCP/IP model has four layers.
- TCP is connection-oriented, while UDP is connectionless.
- Protocol numbers tell receiving devices how to handle information in an IP packet.
- Packet sniffing involves capturing and inspecting network packets.

## Knowledge Check

**Score: 100% ✅**

## Progress

**Module 1 — In Progress**

Today's learning completed successfully. ✅
