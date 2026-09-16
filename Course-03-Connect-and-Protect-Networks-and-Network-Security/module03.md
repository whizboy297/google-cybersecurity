# Module 3 — Secure Against Network Intrusions

**Date:** September 16, 2026  
**Course:** Connect and Protect: Networks and Network Security  
**Module:** Secure Against Network Intrusions

## What I Learned

This module focused on network security, network intrusion tactics, and protecting networks against common attacks.

---

## 1. Network Security

Network security involves protecting networks, systems, and data from unauthorized access and malicious activity.

A security analyst needs to understand how network traffic behaves so that unusual activity can be identified and investigated.

---

## 2. Denial of Service (DoS)

A Denial of Service (DoS) attack attempts to overwhelm a network or server so that normal operations cannot continue.

### Distributed Denial of Service (DDoS)

A DDoS attack uses multiple devices or servers, often from different locations, to flood a target with unwanted traffic.

**Key difference:**

- DoS → attack against a target
- DDoS → multiple devices/hosts are used to attack the target

---

## 3. SYN Flood Attack

A SYN flood attack takes advantage of the TCP connection process.

The attacker sends a large number of SYN packets, simulating the first step of the TCP handshake.

This can overwhelm the server and prevent it from handling legitimate connections.

**Key idea:**

`SYN flood → TCP → excessive SYN requests`

---

## 4. ICMP Flood Attack

An ICMP flood attack overwhelms a system by repeatedly sending ICMP packets.

It takes advantage of the ICMP communication protocol to generate excessive traffic.

---

## 5. Ping of Death

A Ping of Death attack involves sending an oversized ICMP packet to a target.

The course describes an IPv4 ICMP packet larger than 64 KB as an example of the oversized packet used in this attack.

**Key idea:**

`Ping of Death → oversized ICMP packet`

---

## 6. Packet Sniffing

Packet sniffing involves capturing and inspecting data packets while they travel across a network.

### Passive Packet Sniffing

Passive packet sniffing involves reading data packets while they are in transit.

### Active Packet Sniffing

Active packet sniffing involves manipulating data packets while they are in transit.

This can include redirecting packets to unintended ports or changing information contained in the packet.

**Memory aid:**

- Passive = read
- Active = manipulate

### Protection

Using a VPN can help protect data from malicious packet sniffing by encrypting data as it travels across a network.

---

## 7. IP Spoofing

IP spoofing occurs when an attacker changes the source IP address of a data packet to impersonate an authorized system.

The goal can be to make malicious traffic appear to come from a trusted source.

---

## 8. On-Path Attacks

An on-path attack occurs when an attacker positions themselves between communicating systems.

The attacker can intercept traffic between a web browser and a web server and potentially inspect or manipulate the communication.

---

## 9. Replay Attacks

A replay attack occurs when an attacker intercepts a data packet and later delays or repeats it.

**Key idea:**

`Replay → capture → delay/repeat`

---

## 10. Smurf Attacks

A smurf attack combines characteristics of a DDoS attack and IP spoofing.

The attacker spoofs an authorized user's IP address and floods the target with packets.

**Key idea:**

`Smurf attack → DDoS + IP spoofing`

---

## 11. Network Traffic Analysis

I also practiced analyzing network traffic using `tcpdump`.

In the network incident involving `www.yummyrecipesforme.com`, the DNS request was sent using UDP to port 53.

The response contained an ICMP error:

`udp port 53 unreachable`

This indicated that the DNS request could not reach a service listening on UDP port 53.

This demonstrated how a security analyst can inspect packet data to identify network-related problems during a security incident.

---

## Key Takeaways

- DoS attacks overwhelm a target and disrupt normal operations.
- DDoS attacks use multiple devices or hosts.
- SYN floods target the TCP connection process.
- ICMP floods generate excessive ICMP traffic.
- Ping of Death uses an oversized ICMP packet.
- Passive packet sniffing reads traffic.
- Active packet sniffing manipulates traffic.
- IP spoofing changes the source IP to impersonate another system.
- On-path attacks intercept communication between systems.
- Replay attacks delay or repeat intercepted packets.
- Smurf attacks combine DDoS and IP spoofing.
- `tcpdump` can be used to inspect network traffic during investigations.

## Assessment Result

**Highest score: 97.5% ✅**

**Module 3 completed — September 16, 2026.**
