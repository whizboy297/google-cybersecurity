# Module 4 — Security Hardening

**Date:** Tuesday, 13 October 2026  
**Course:** Google Cybersecurity Professional Certificate  
**Course 3:** Connect and Protect: Networks and Network Security

## Lessons Completed

- Security hardening
- Operating system (OS) hardening
- Network hardening practices
- Cloud network hardening
- Security risk assessment
- Incident report analysis using the NIST Cybersecurity Framework (CSF)
- Security hardening knowledge checks and assessment

---

## 1. Security Hardening

Security hardening is the process of strengthening systems to reduce vulnerabilities and minimise the attack surface.

The purpose is to make it more difficult for threat actors to exploit weaknesses in systems, networks, and cloud environments.

Security hardening involves applying appropriate security controls, updating software, restricting access, disabling unnecessary services, and monitoring systems for suspicious activity.

### Why Security Hardening Matters

- Reduces the attack surface.
- Helps prevent attackers from exploiting known vulnerabilities.
- Restricts unauthorised access.
- Improves system and network security.
- Reduces the potential impact of a successful attack.

**Key takeaway:** Security hardening reduces security risks by removing unnecessary exposure and addressing vulnerabilities.

---

## 2. Operating System (OS) Hardening

OS hardening involves securing an operating system by addressing vulnerabilities, controlling user permissions, protecting credentials, and removing unnecessary applications and services.

### OS Hardening Techniques

**1. Patch Updates**

Regularly updating operating systems and software helps fix known security vulnerabilities.

Security patches address weaknesses that attackers might otherwise exploit.

**2. Principle of Least Privilege**

The principle of least privilege means giving users and processes only the minimum permissions required to perform their tasks.

For example, an ordinary employee should not automatically have administrator privileges.

If an attacker compromises an account with limited permissions, the attacker's ability to access other resources or make system-wide changes is restricted.

**3. Multifactor Authentication (MFA)**

MFA requires users to verify their identity using at least two different authentication factors.

The factors can include:

- Something you know, such as a password.
- Something you have, such as a security token.
- Something you are, such as a fingerprint.

MFA adds another layer of protection if a password is stolen or guessed.

**4. Removing Unnecessary Applications and Services**

Unused applications and services should be removed or disabled where appropriate.

Every unnecessary running service may create another potential entry point for attackers.

Removing these components helps reduce the attack surface.

**5. Baseline Configuration**

A baseline configuration is an approved reference configuration for a system.

Security professionals can compare the current configuration against the approved baseline to identify unauthorised changes or security weaknesses.

For example, an analyst might compare the current firewall settings with the organisation's documented security requirements.

### What I Learned

OS hardening focuses on protecting the operating system, its applications, its services, and the permissions assigned to users and processes.

Least privilege is particularly important because it helps limit the damage an attacker can cause if an account is compromised.

---

## 3. Network Hardening Practices

Network hardening involves securing network infrastructure, connections, and traffic to reduce vulnerabilities and prevent unauthorised access.

### 3.1 Port Filtering

Port filtering controls which network ports are allowed to communicate.

The principle is to allow ports required for normal network operations and block or disable unnecessary ports.

For example, if a server does not need a particular service, its associated port should not be unnecessarily exposed.

**Purpose:** Reduces the attack surface by limiting unnecessary network entry points.

### 3.2 Network Segmentation

Network segmentation divides a network into separate sections or subnets.

Different departments or systems can be placed in separate segments, with access controlled according to their requirements.

For example, a company could separate its HR, Finance, and IT networks.

If an attacker compromises one segment, segmentation can make it more difficult to move laterally into other parts of the network.

**Purpose:** Restricts access between network areas and helps contain security incidents.

### 3.3 Intrusion Detection and Prevention Systems (IDS/IPS)

An Intrusion Detection System (IDS) monitors network activity to identify suspicious behaviour and generate alerts.

An Intrusion Prevention System (IPS) can take action to block certain malicious or suspicious traffic according to its configuration.

These systems help security teams detect and respond to potential attacks.

**Purpose:** Identifies suspicious activity and can help prevent malicious traffic from reaching protected systems.

### 3.4 Secure Protocols

Secure protocols help protect information transmitted across networks.

Examples include:

- **HTTPS:** Protects communication between web browsers and web servers using encryption.
- **SSH:** Provides an encrypted method for remotely accessing and administering systems.

Encryption helps prevent unauthorised parties from reading intercepted data.

**Purpose:** Reduces the risk of eavesdropping and protects data in transit.

### 3.5 SIEM Tools

Security Information and Event Management (SIEM) tools collect and analyse log data from systems, applications, and network devices.

Examples include Splunk.

Security analysts can use SIEM tools to investigate suspicious activities, such as repeated failed login attempts or unusual network traffic.

**Purpose:** Improves visibility into security events and supports incident investigation.

### 3.6 Security Audits and Penetration Testing

**Security audits**

Security audits involve reviewing security controls, configurations, policies, and procedures to identify gaps or deviations from requirements.

**Penetration testing**

Penetration testing involves simulating attacks against systems within an authorised scope to identify exploitable vulnerabilities.

The results help organisations understand weaknesses and decide which corrective measures are needed.

**Key takeaway:** Audits review security arrangements, while penetration testing attempts to identify exploitable weaknesses.

---

## 4. Cloud Network Hardening

Cloud network hardening involves securing cloud-hosted resources and controlling how they communicate with other systems.

### Security Groups

Security groups act like virtual firewalls for cloud resources.

They use rules to control permitted incoming and outgoing network traffic.

For example, a company could configure a cloud database to accept connections only from an authorised application server.

This reduces unnecessary exposure and helps prevent unauthorised connections.

### What I Learned

Cloud security groups help enforce network access rules around cloud resources.

They are similar to firewalls because they control traffic, but their configuration and scope depend on the cloud platform.

---

## 5. Security Risk Assessment: Social Media Organisation

The activity described a social media organisation that had experienced a major data breach.

The security team identified four vulnerabilities:

1. Employees shared passwords.
2. The database administrator password was still set to the default.
3. Firewalls lacked rules for filtering incoming and outgoing traffic.
4. Multifactor authentication was not being used.

### Recommended Security Measures

**Shared passwords**

Give every employee an individual account and enforce policies against password sharing.

Individual accounts improve accountability and help security teams identify which account performed an action.

**Default database administrator password**

Replace the default password with a strong, unique credential.

Restrict administrative access to authorised personnel and store credentials securely.

**Missing firewall rules**

Configure firewall rules to allow only necessary, authorised traffic.

Use port filtering to block unnecessary ports and review firewall configurations regularly.

**Absence of MFA**

Implement MFA for employee accounts, especially accounts with privileged access to sensitive information.

MFA adds an extra layer of verification if a password is compromised.

**Additional protection**

Network segmentation can restrict access to sensitive systems, while security monitoring can help identify suspicious activities.

### Important Distinction

Network segmentation does not directly prevent employees from sharing passwords.

Individual accounts and appropriate authentication policies address password sharing more directly, while segmentation restricts communication between network areas.

---

## 6. Incident Report Analysis: ICMP Flooding Attack

### Incident Summary

A multimedia company providing web design, graphic design, and social media marketing services experienced a denial-of-service (DoS) attack.

The attacker flooded the company's network with ICMP packets, causing network services to stop responding for approximately two hours.

The investigation identified an unconfigured firewall as the vulnerability that allowed the malicious traffic to enter the network.

The incident management team responded by blocking incoming ICMP packets, stopping non-critical network services, and restoring critical services.

The organisation then implemented additional security measures:

- A firewall rule to limit the rate of incoming ICMP packets.
- Source IP address verification to check for spoofed IP addresses.
- Network monitoring software to detect abnormal traffic patterns.
- An IDS/IPS system to filter ICMP traffic based on suspicious characteristics.

### 6.1 Identify

The Identify function involves understanding the incident, identifying affected resources, and determining the security risks.

In this scenario:

- The attack involved an ICMP flood.
- Internal network services became unresponsive.
- An unconfigured firewall allowed the malicious traffic to enter.
- The affected services and network resources needed to be identified and assessed.

### 6.2 Protect

The Protect function focuses on implementing safeguards to reduce the likelihood and impact of future attacks.

Recommended measures include:

- Configuring firewall rules to limit incoming ICMP traffic.
- Implementing IDS/IPS protection.
- Reviewing firewall configurations regularly.
- Restricting unnecessary network exposure.
- Maintaining documented security configurations.

These measures help reduce the likelihood of another ICMP flood overwhelming the network.

### 6.3 Detect

The Detect function involves monitoring systems and network traffic to identify potential security incidents.

Recommended measures include:

- Monitoring incoming ICMP traffic.
- Detecting abnormal traffic patterns.
- Verifying source IP addresses to help identify spoofed traffic.
- Reviewing firewall and IDS/IPS logs.
- Establishing normal traffic baselines.
- Configuring alerts for unusual increases in network activity.

These practices help security analysts identify potential attacks earlier.

### 6.4 Respond

The Respond function focuses on containing and investigating security incidents.

A response plan should include:

1. Confirming the attack and assessing affected services.
2. Applying firewall restrictions and other containment measures.
3. Isolating affected systems when necessary.
4. Analysing network traffic, firewall logs, and IDS/IPS alerts.
5. Informing the incident management team and relevant stakeholders.
6. Documenting the incident and actions taken.
7. Reviewing the incident to identify improvements.

The aim is to limit the impact, understand the cause, and prevent further disruption.

### 6.5 Recover

The Recover function focuses on restoring affected systems and services to normal operation.

Recommended recovery steps include:

- Restoring critical network services first.
- Verifying that restored services function correctly.
- Monitoring network traffic and performance.
- Bringing non-critical services back online when safe.
- Reviewing the incident response and recovery procedures.
- Implementing improvements to reduce the risk of recurrence.

**Terminology note:** The scenario describes a DoS attack. A distributed denial-of-service (DDoS) attack involves multiple sources or systems; the scenario does not confirm that multiple attacking systems were involved.

---

## 7. NIST Cybersecurity Framework (CSF)

The incident report activity used five NIST CSF functions.

| Function | Purpose |
|---|---|
| Identify | Understand cybersecurity risks and identify affected systems and resources. |
| Protect | Implement safeguards to reduce cybersecurity risks. |
| Detect | Identify suspicious activity and potential security incidents. |
| Respond | Contain, investigate, and manage security incidents. |
| Recover | Restore affected systems and improve recovery procedures. |

### My Understanding

The five functions work together to help organisations manage cybersecurity risks.

For example, when a network attack occurs, the organisation identifies the problem, applies protective measures, detects suspicious activity, responds to the incident, and restores normal operations.

The lessons learned from the incident can then be used to strengthen security controls.

---

## 8. Key Cybersecurity Terms

- **Attack surface:** The potential points through which an attacker could attempt to access or affect a system.
- **Baseline configuration:** An approved reference configuration used to check current system settings.
- **DoS:** A denial-of-service attack that disrupts the availability of a service or network.
- **ICMP:** Internet Control Message Protocol, used for network messages and diagnostics.
- **IDS:** An Intrusion Detection System that monitors activity for suspicious behaviour.
- **IPS:** An Intrusion Prevention System that can block certain malicious traffic.
- **Least privilege:** Giving users and processes only the permissions they need.
- **MFA:** Authentication that requires at least two different authentication factors.
- **Network segmentation:** Dividing a network into separate sections with controlled communication.
- **Port filtering:** Allowing or blocking network traffic based on port rules.
- **SIEM:** Technology that collects and analyses security logs and events.
- **Penetration testing:** Authorised simulated attacks used to identify exploitable vulnerabilities.
- **Security audit:** A review of security controls, configurations, policies, and procedures.

---

## 9. Assessment Results

| Activity | Score or status |
|---|---|
| Security hardening knowledge check | 93.75% |
| Network hardening knowledge check | 100% |
| Security hardening assessment | 100% |
| Course 3 certificate | Completed |

**Certificate:** Connect and Protect: Networks and Network Security  
**Completion date:** 13 October 2026

---

## 10. My Reflection

Today I learned that security hardening involves using different controls to address specific vulnerabilities.

I learned that patch updates fix known software vulnerabilities, least privilege limits what a compromised account can do, and port filtering reduces unnecessary network exposure. Network segmentation helps restrict communication between systems, while MFA provides an additional layer of account protection.

I also learned how SIEM tools, IDS/IPS systems, and network monitoring software support the detection and investigation of suspicious activity.

The incident report activity helped me apply the NIST Cybersecurity Framework to an ICMP flooding incident. I learned how Identify, Protect, Detect, Respond, and Recover can be used together to manage an incident and improve an organisation's security.

These concepts provide a foundation for further cybersecurity study and future work in security analysis.

---

## Summary

Module 4 focused on security hardening across operating systems, networks, and cloud environments.

I learned how to reduce the attack surface, restrict access, monitor suspicious activity, and apply appropriate controls to specific vulnerabilities. I also practised using the NIST Cybersecurity Framework to analyse a network incident and recommend measures for protection, detection, response, and recovery.

These skills are important foundations for understanding how cybersecurity professionals protect systems, investigate incidents, and improve an organisation's security posture.
