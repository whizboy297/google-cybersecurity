# Day 3 — SIEM, Security Tools & Incident Response

**Date:** September 2, 2026  
**Course:** Play It Safe: Manage Security Risks

## What I Learned

Today I learned about SIEM tools, security logs, dashboards, open-source and proprietary security tools, SIEM deployment types, and incident response playbooks.

---

## 1. Security Logs

Server logs record events related to services and systems.

Examples include:

- Website activity
- Email activity
- File shares
- Login requests
- Username and password requests
- Ongoing service use

Logs provide important information that security teams can analyze when investigating security events.

---

## 2. SIEM

SIEM stands for:

**Security Information and Event Management**

SIEM tools collect and analyze log data to help security teams monitor critical activities.

They help analysts identify suspicious activity without having to manually review every individual log.

---

## 3. Security Metrics

Metrics are key technical attributes used to evaluate software and system performance.

Examples include:

- Response time
- Availability
- Failure rate

SIEM tools and dashboards can use metrics to help security teams understand system activity and performance.

---

## 4. SIEM Dashboards

SIEM dashboards provide visual information that helps security analysts monitor and investigate security events.

### Security Posture Dashboard

Used by Security Operations Centers (SOCs) to monitor notable security events and trends.

### Executive Summary Dashboard

Provides high-level information about an organization's overall security health over time.

### Incident Review Dashboard

Helps analysts identify suspicious patterns surrounding security incidents.

### Risk Analysis Dashboard

Shows risk associated with objects such as:

- Users
- Computers
- IP addresses

---

## 5. Open-Source vs Proprietary Security Tools

### Open-Source

Open-source tools make their source code publicly available and can often be customized or modified according to their license.

Examples:

- Linux
- Suricata

### Proprietary

Proprietary tools are owned and controlled by a company or individual. Their source code is generally restricted.

Examples:

- Splunk
- Google SecOps (Chronicle)

Open-source tools are not automatically less secure than proprietary tools.

---

## 6. SIEM Deployment Types

### Self-Hosted

The organization hosts and manages the SIEM itself.

### Cloud-Hosted

The SIEM is hosted in the cloud, providing flexibility and scalability.

### Hybrid

Combines self-hosted and cloud-hosted environments.

### Cloud-Native

Designed specifically to take advantage of cloud capabilities.

---

## 7. Chronicle

Google SecOps (Chronicle) is a cloud-native SIEM.

It can retain, analyze, and search logs to identify threats, risks, and vulnerabilities.

Chronicle can analyze information by:

- Asset
- Domain name
- User
- IP address

Examples of Chronicle dashboards include:

- Enterprise insights
- Data ingestion and health
- IOC matches
- Main dashboard
- Rule detections
- User sign-in overview

---

## 8. Incident Response Playbooks

Playbooks are living documents that provide structured procedures for responding to security incidents.

They should be updated regularly based on:

- Previous security incidents
- New threats
- New vulnerabilities
- Lessons learned

### Incident Response Phases

1. **Preparation** — Get people, procedures, and resources ready.
2. **Detection and Analysis** — Investigate alerts and determine what happened.
3. **Containment** — Limit the incident and prevent further damage.
4. **Eradication and Recovery** — Remove the threat and restore affected systems.
5. **Post-Incident Activity** — Analyze what happened and identify improvements.
6. **Coordination** — Share information with relevant stakeholders according to established standards.

---

## Key Takeaways

- Logs provide valuable information about system and user activity.
- SIEM tools collect and analyze logs to help identify security events.
- Dashboards help analysts visualize security activity and risks.
- Open-source and proprietary tools have different ownership and customization models.
- SIEM systems can be self-hosted, cloud-hosted, hybrid, or cloud-native.
- Chronicle is a cloud-native SIEM.
- Playbooks provide structured guidance for responding to security incidents.
- Playbooks should evolve as organizations learn from previous incidents.
- Incident response involves preparation, detection, containment, eradication and recovery, post-incident activity, and coordination.

## Progress

**Day 3 completed — 100% on knowledge checks. ✅**

**Course 2 completed — Final grade: 92.57%. 🎓**
