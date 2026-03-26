---
layout: default
---

# Incident Response Playbook
### Cybersecurity Bootcamp Capstone &nbsp;|&nbsp; September 2025

[Back to Portfolio](./index.html)

* * *

## Objective

Develop a comprehensive Incident Response Playbook for phishing and Business Email Compromise (BEC) attacks targeting a banking institution — built using the NIST Incident Response Framework and informed by findings from the OSINT and Risk Assessment capstones.

* * *

## Why This Risk Was Selected

During the risk assessment, executive-targeted phishing was identified as the highest priority risk with a score of 16 — Likelihood 4 (High), Impact 4 (High). Three key factors drove this selection:

- The OSINT assessment identified 38 named executives with publicly accessible roles and reporting structures — providing attackers with a ready-made spear-phishing target list
- Regulatory documentation from TTSEC and the Central Bank of Barbados is publicly accessible — enabling realistic regulatory impersonation attacks
- The Finance department's access to the PCI DSS payment database (VLAN 110) means compromised credentials could lead to immediate financial fraud

* * *

## Response Teams

| Team | Composition | Primary Role |
|:---|:---|:---|
| Security Operations Center (SOC) | SOC Manager, 3 Security Analysts, Threat Intelligence Analyst, Forensic Investigator | Continuous monitoring, triage, alert generation, documentation |
| Incident Response Team (IRT) | IR Manager, Security Operations Lead, Legal Counsel, Communications Director, Compliance Officer | Decision making, regulatory compliance, stakeholder communications, risk management |
| IT & Identity Management Team | IT Manager, 2 Network Engineers, 3 Systems Administrators, Database Administrator | Credential management, access control, MFA enforcement, recovery support |

* * *

## NIST Incident Response Phases

---

### Phase 1 — Preparation

Establish all people, processes, and technology needed to detect and respond to phishing attacks before they occur.

**Key Actions:**
- Configure Cisco Email Security Appliance rules to detect phishing patterns — homograph domains, display name spoofing, urgent language
- Deploy SIEM correlation rules to detect anomalies — multiple executives receiving similar emails, logins from unusual locations, access outside business hours
- Assign defined roles across SOC, IT Infrastructure, and Executive Communications teams
- Implement network segmentation separating Management VLAN (192.168.10.0/24) and Finance VLAN (192.168.20.0/24) from PCI DSS Database (VLAN 110) and PII Database (VLAN 120)
- Develop Central Bank of Barbados breach notification templates for 72-hour regulatory requirement

---

### Phase 2 — Detection and Analysis

Rapidly identify phishing attacks, assess scope and impact, and gather forensic evidence.

**Key Actions:**
- Monitor Cisco Email Security Appliance alerts and SIEM correlation logs for suspicious authentication activity
- Analyse user-reported suspicious emails forwarded to security inbox
- Correlate with FS-ISAC threat intelligence feeds and Barbados Bankers Association security bulletins
- Perform memory dumps of affected executive workstations using EnCase or FTK Imager
- Query Database Activity Monitoring logs to identify any access to PCI DSS Database (VLAN 110) or PII Database (VLAN 120) by compromised accounts

---

### Phase 3 — Containment

Immediately stop phishing attack progression and prevent further credential abuse.

**Key Actions:**
- Activate Cisco Email Security Appliance emergency rules to block phishing sender domains and IP addresses
- Isolate compromised executive accounts in Active Directory while maintaining forensic integrity
- Implement Conditional Access policies restricting compromised accounts from accessing databases and VPN
- Activate Data Loss Prevention systems to block customer data from leaving the network
- Implement manual approval workflow for wire transfers exceeding $50,000 USD during the incident

---

### Phase 4 — Eradication and Recovery

Eliminate the phishing threat and restore safe banking operations.

**Key Actions:**
- Deploy full DMARC policy for the bank's domain to prevent spoofed emails from reaching users
- Reset passwords for all 38 executives using verified clean procedures with new complexity requirements
- Verify integrity of all systems accessed by compromised accounts — scan for malware, web shells, and backdoors
- Conduct penetration testing on restored Exchange systems, Azure AD, and online banking applications
- Validate all third-party integrations and correspondent banking system connections

---

### Phase 5 — Post-Incident

Comprehensive analysis, regulatory reporting, and security improvement.

**Key Actions:**
- Submit formal incident report to Central Bank of Barbados Banking Supervision Department within 72 hours
- File required reports with PCI DSS payment card brands if cardholder data was compromised
- Conduct root cause analysis using the 5 Whys technique
- Share anonymised lessons learned with Barbados Bankers Association and FS-ISAC
- Update the playbook incorporating lessons learned and enhanced detection procedures

* * *

## Tools Specified

| Tool | Purpose | Phase Used |
|:---|:---|:---|
| Splunk Enterprise Security | SIEM — log correlation and suspicious pattern detection | Detection, Containment, Post-Incident |
| CrowdStrike Falcon | EDR — endpoint monitoring and credential theft detection | Detection, Containment, Eradication |
| Cisco Email Security Appliance | Email gateway — phishing detection and quarantine | Preparation, Detection, Containment |
| KnowBe4 | Security awareness training and phishing simulations | Preparation, Post-Incident |
| RSA SecurID | MFA for executives and privileged users | Containment, Recovery |

* * *

## Regulatory Communication Plan

**Central Bank of Barbados — Banking Supervision Department**
- Notification required within 72 hours of discovery
- Method: Encrypted email to Banking Supervision contact, followed by registered mail to Tom Adams Financial Centre, Bridgetown
- In-person briefing with senior supervisors within 48 hours

**TTSEC — Trinidad and Tobago Securities and Exchange Commission**
- Required if incident affects Republic Financial Holdings Limited parent company operations
- Method: Formal written notification through TTSEC regulatory filing portal, followed by telephone confirmation with Compliance Division

* * *

## Key Takeaway

Documentation is a massive part of security work. Building this playbook demonstrated that an effective incident response is not reactive — it is built, tested, and refined long before an attack occurs. Every decision made during an incident should have a documented procedure behind it.

* * *

[Back to Portfolio](./index.html)
