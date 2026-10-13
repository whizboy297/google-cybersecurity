# Cybersecurity Projects

This page documents my cybersecurity learning projects, security assessments, incident analysis, and practical exercises as I work towards a career in cybersecurity.

My focus is on developing the foundational skills required for entry-level roles such as Junior SOC Analyst and Cybersecurity Analyst.

---

## Project 1: Security Hardening and Risk Assessment

**Category:** Security Hardening and Risk Management  
**Course:** Google Cybersecurity Professional Certificate — Course 3  
**Date:** October 13, 2026  
**Status:** Completed

### Overview

This exercise focused on identifying security weaknesses in an organisation and recommending appropriate controls to reduce risk.

The assessment considered weaknesses involving employee password practices, default administrator credentials, firewall configurations, and the absence of multifactor authentication.

### Security Weaknesses Identified

- Employees sharing passwords.
- A database administrator account using a default password.
- Missing firewall traffic-filtering rules.
- Lack of multifactor authentication.

### Recommended Security Controls

- Introduce individual user accounts and stronger password policies.
- Replace default credentials with secure, unique passwords.
- Apply the principle of least privilege.
- Configure firewall rules and restrict unnecessary ports.
- Implement multifactor authentication.
- Use network segmentation to limit unnecessary access.
- Monitor systems and network activity for suspicious behaviour.

### Skills Demonstrated

- Security risk assessment.
- Vulnerability identification.
- Security hardening.
- Access control.
- Firewall configuration concepts.
- Risk mitigation.
- Security monitoring.

### Key Learning

Security hardening reduces an organisation's attack surface by removing unnecessary services, strengthening configurations, restricting access, and implementing appropriate security controls.

---

## Project 2: Network Security Incident Report — ICMP Flood DoS

**Category:** Network Security and Incident Response  
**Framework:** NIST Cybersecurity Framework (CSF)  
**Course:** Google Cybersecurity Professional Certificate — Course 3  
**Date:** October 13, 2026  
**Status:** Completed

### Overview

This exercise involved analysing a denial-of-service (DoS) incident affecting a multimedia company's internal network.

Internal network services became unresponsive for approximately two hours. The scenario identified an improperly configured firewall that allowed ICMP packets without appropriate restrictions.

### Incident Analysis

The incident demonstrated how excessive ICMP traffic can affect network availability when traffic controls are inadequate.

The firewall configuration was identified as a contributing weakness. The response focused on limiting the unwanted traffic, restoring essential services, and improving network defences.

### Response and Mitigation Measures

- Block incoming ICMP traffic where appropriate.
- Apply ICMP rate limiting to control excessive traffic.
- Verify source IP information as part of investigating potentially spoofed traffic.
- Monitor network traffic for unusual patterns.
- Use IDS/IPS capabilities to help detect suspicious activity.
- Stop non-critical services where necessary to support recovery.
- Restore critical services and verify their availability.
- Review firewall rules to prevent similar incidents.

### NIST Cybersecurity Framework

The incident was analysed using the five NIST CSF functions:

| Function | Application |
|---|---|
| Identify | Identify the affected services, network weaknesses, and potential risks. |
| Protect | Strengthen firewall rules and introduce appropriate traffic controls. |
| Detect | Monitor network activity and look for unusual ICMP traffic patterns. |
| Respond | Restrict unwanted traffic and take steps to restore essential services. |
| Recover | Restore critical services and improve defences to reduce the likelihood of recurrence. |

### Skills Demonstrated

- Network security analysis.
- Denial-of-service incident analysis.
- Firewall security concepts.
- Network monitoring.
- Incident response planning.
- Security mitigation.
- NIST Cybersecurity Framework application.

### Key Learning

Network availability depends on effective traffic management, secure firewall configurations, monitoring, and a structured incident response process.

---

## Project 3: Network and System Security Hardening

**Category:** Network Security and Defensive Security  
**Course:** Google Cybersecurity Professional Certificate — Course 3  
**Date:** October 13, 2026  
**Status:** Completed

### Overview

This exercise explored security hardening techniques for operating systems, networks, and cloud environments.

The objective was to understand how secure configurations and defensive controls can reduce vulnerabilities and limit opportunities for attackers.

### Hardening Techniques Reviewed

#### Operating System Security

- Apply operating system and software updates.
- Remove unnecessary applications and services.
- Enforce least-privilege access.
- Require multifactor authentication where appropriate.
- Review system configurations against security baselines.

#### Network Security

- Restrict unnecessary ports and network traffic.
- Configure firewall rules.
- Use network segmentation to separate systems and limit unnecessary communication.
- Use secure communication protocols such as HTTPS and SSH.
- Monitor network activity for suspicious behaviour.

#### Cloud Security

- Use cloud security groups to control inbound and outbound traffic.
- Restrict access to cloud resources.
- Allow only the network traffic required for legitimate operations.

#### Security Monitoring and Assessment

- Use SIEM tools to collect and analyse security events.
- Understand the role of IDS/IPS in detecting and preventing suspicious activity.
- Conduct security audits.
- Use authorised penetration testing to identify weaknesses.

### Skills Developed

- Operating system hardening concepts.
- Network hardening.
- Cloud security fundamentals.
- Firewall and port-filtering concepts.
- Network segmentation.
- SIEM fundamentals.
- IDS/IPS fundamentals.
- Security assessment.

### Key Learning

Effective security hardening combines secure configurations, access restrictions, traffic controls, regular updates, and continuous monitoring.

---

## Learning Resources and Supporting Evidence

These projects were completed as part of the Google Cybersecurity Professional Certificate.

- [Course 3 — Connect and Protect: Networks and Network Security](../Course-03-Connect-and-Protect-Networks-and-Network-Security/)
- [Course Certificates](certificates/README.md)
- [Certifications Overview](certifications.md)

---

## Future Projects

I intend to expand this portfolio with additional projects involving:

- Linux security and command-line investigations.
- Network traffic analysis using Wireshark.
- SIEM investigations and security alert analysis.
- Log analysis and incident investigation.
- Python scripting for security tasks.
- Vulnerability assessment in authorised lab environments.
- Incident response documentation and security playbooks.

These projects will be added as I complete the relevant exercises and develop further practical experience.
