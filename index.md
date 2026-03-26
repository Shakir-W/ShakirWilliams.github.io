---
layout: default
---

# Shakir Williams
### Cloud Security | DevSecOps | Network Administration

📍 Barbados &nbsp;|&nbsp; 📧 shakirwilliams07@gmail.com &nbsp;|&nbsp; [LinkedIn](https://linkedin.com/in/[Your-LinkedIn]) &nbsp;|&nbsp; [GitHub](https://github.com/[Your-GitHub])

> CompTIA Security+ Certified &nbsp;|&nbsp; BSc Computer Science & Electronic Engineering – University of the West Indies &nbsp;|&nbsp; Cybersecurity Bootcamp Graduate

* * *

## About Me

I am an emerging Cloud Security and DevSecOps professional based in Barbados with hands-on experience in network administration, cybersecurity risk assessment, vulnerability analysis, and incident response planning. I have practical experience working as a Junior Network Administrator at the Barbados Transport Board, where I configured network systems and delivered the GoCity Card integration project — connecting student databases to bus driver tablets and card readers across Barbados.

I completed a Cybersecurity Bootcamp producing four professional-grade capstone projects applied to real Caribbean financial institutions covering OSINT investigation, risk assessment, enterprise network design, and incident response. I am currently pursuing a Bachelor's Degree in Computer Science and Electronic Engineering at the University of the West Indies.

My focus is on securing cloud environments, automating security remediation, and integrating security into every stage of the development lifecycle.

* * *

## Certifications

| Certification | Issuer | Status |
|:---|:---|:---|
| CompTIA Security+ (SY0-701) | CompTIA | ✅ Completed |
| AWS Cloud Practitioner | Amazon Web Services | 🎯 In Progress |
| AWS Solutions Architect Associate | Amazon Web Services | 🎯 Planned |

* * *

## Technical Skills

### Cloud & DevSecOps
- Amazon Web Services (AWS) — cloud infrastructure and resource management
- AWS Security Hub — identifying and remediating security risks across cloud environments
- Amazon Inspector — vulnerability detection and reporting across cloud instances
- Infrastructure as Code (IaC) — AWS CloudFormation, Terraform, YAML
- DevSecOps — integrating security controls across development, testing, and deployment pipelines
- Security Posture Management — improving cloud security posture using NIST, PCI DSS, and SOC frameworks

### Security & Analysis
- Vulnerability Assessment & Risk Management — NIST, COBIT 2019, PCI DSS, SOC, COSO frameworks
- OSINT & Threat Intelligence — multi-platform open-source intelligence gathering and analysis
- Incident Response — NIST IR phases, playbook development, regulatory communication planning
- Security Tools — Splunk (SIEM), CrowdStrike Falcon (EDR), Qualys, KnowBe4, RSA SecurID MFA

### Networking & Infrastructure
- Network Administration — configuring, setting up, and maintaining network systems
- Network Security — VLAN segmentation, ACL firewall rules, enterprise topology design
- Cisco Packet Tracer — enterprise banking network design and simulation
- Technical Troubleshooting — diagnosing and resolving hardware, software, and network issues

### Other
- Python — scripting and automation fundamentals
- Database Management — data entry, organisation, and system integration
- Documentation — professional report writing, playbook development, regulatory reporting

* * *

## Cybersecurity Projects

* * *

### OSINT Investigation
`August 2025` &nbsp;|&nbsp; `Cybersecurity Bootcamp` &nbsp;|&nbsp; `Barbados`

**Objective:** Conduct a comprehensive Open-Source Intelligence investigation on a senior banking executive at Republic Bank Barbados using only publicly available sources to identify what sensitive information was exposed and how threat actors could exploit it.

**What Was Done:**
- Identified and classified **5 categories of sensitive information** with sensitivity ratings from Medium to Critical
- Analysed **5 threat actor exploitation methods** — social engineering, spear-phishing, network infiltration, regulatory impersonation, and strategic intelligence exploitation
- Applied 3 OSINT methodologies — corporate database mining, cross-platform network analysis, and search engine media analysis

**Sensitive Information Identified:**

| Category | Sensitivity |
|:---|:---|
| Professional career timeline & employer history | HIGH |
| Organisational structure & executive network | MEDIUM-HIGH |
| Public speaking engagements & community participation | HIGH |
| Business direction & development intelligence | CRITICAL |
| Regulatory and compliance documentation | HIGH |

**Tools & Sources Used:**
- LinkedIn, Facebook, Twitter, Instagram
- TTSEC corporate databases and executive org charts
- Barbados Today, Guyana Chronicle, Trinidad-based publications
- ZoomInfo, TheOfficialBoard

📄 [View Full Report](https://github.com/[Your-GitHub]/OSINT-Capstone)

* * *

### Cybersecurity Risk Assessment
`September 2025` &nbsp;|&nbsp; `Cybersecurity Bootcamp` &nbsp;|&nbsp; `Barbados`

**Objective:** Perform a full cybersecurity risk assessment on Republic Bank (Barbados) Limited based on OSINT findings, identifying organisational vulnerabilities, scoring them by likelihood and impact, and developing actionable recommendations.

**What Was Done:**
- Identified and assessed **5 organisational vulnerabilities** with severity ratings from Low-Medium to Critical
- Produced a **scored risk matrix** with likelihood and impact analysis across all identified risks
- Applied 4 industry frameworks to the assessment
- Developed actionable recommendations for the 2 highest priority asset categories

**Risk Matrix Results:**

| Risk | Likelihood | Impact | Priority |
|:---|:---|:---|:---|
| Executive Leadership & Org Structure Exploitation | 4 – High | 4 – High | HIGH |
| Regulatory Documentation Exploitation | 3 – Medium | 5 – Critical | CRITICAL IMPACT |
| Strategic Communications Intelligence | 3 – Medium | 3 – Medium | MEDIUM |
| Third-Party Relationship Intelligence | 3 – Medium | 2 – Low-Medium | LOW-MEDIUM |
| Corporate Communications Exploitation | 4 – High | 2 – Low-Medium | LOW-MEDIUM |

**Frameworks Applied:**
- NIST Cybersecurity Framework | COBIT 2019 | COSO Internal Control Framework | PCI DSS & SOC

📄 [View Full Report](https://github.com/[Your-GitHub]/Risk-Assessment-Capstone)

* * *

### Enterprise Network Design
`September 2025` &nbsp;|&nbsp; `Cybersecurity Bootcamp` &nbsp;|&nbsp; `Barbados`

**Objective:** Design and build a full secure enterprise network topology for a banking organisation meeting PCI DSS compliance requirements using Cisco Packet Tracer.

**What Was Done:**
- Designed a complete enterprise banking network with **8 department VLANs**
- Configured multilayer switches, DHCP/DNS/Mail/Application servers, and banking database infrastructure
- Wrote and justified **5 ACL firewall rules** enforcing least-privilege access
- Documented full security theory covering availability, data protection, and attack surface limitation

**Network Architecture:**

| VLAN | Department | Subnet |
|:---|:---|:---|
| VLAN 10 | Management | 192.168.10.0/24 |
| VLAN 20 | Finance | 192.168.20.0/24 |
| VLAN 30 | Public Relations | 192.168.30.0/24 |
| VLAN 40 | IT Department | 192.168.40.0/24 |
| VLAN 50 | R&D | 192.168.50.0/24 |
| VLAN 60 | Guest Network | 192.168.60.0/24 |
| VLAN 110 | PCI DSS Payment Database | 192.168.110.0/24 |
| VLAN 120 | PII Customer Database | 192.168.120.0/24 |

**Firewall Rules Written:**

| Rule | Purpose |
|:---|:---|
| Rule 1 | Block external access to database ports — SQL Server 1433, MySQL 3306, PostgreSQL 5432 |
| Rule 2 | Time-based management access — HTTPS permitted during business hours only |
| Rule 3 | Block guest network from accessing PCI DSS and PII databases |
| Rule 4 | Allow Finance VLAN secure HTTPS access to payment systems only |
| Rule 5 | Force all outbound traffic through proxy for content filtering and malware scanning |

**Security Technologies Implemented:**
- HSRP failover, Spanning Tree Protocol Rapid-PVST+, dual ISP BGP routing
- AES-256 encryption, TLS 1.3, Hardware Security Module (HSM)
- DMZ for public-facing services, Web Application Firewall (WAF), IPS

📄 [View Full Report](https://github.com/[Your-GitHub]/Network-Design-Capstone)

* * *

### Incident Response Playbook
`September 2025` &nbsp;|&nbsp; `Cybersecurity Bootcamp` &nbsp;|&nbsp; `Barbados`

**Objective:** Develop a comprehensive Incident Response Playbook for phishing and Business Email Compromise (BEC) attacks targeting a banking institution using the NIST Incident Response Framework.

**What Was Done:**
- Defined roles and responsibilities for **3 response teams**
- Documented all **5 NIST incident response phases** with specific actions, tools, and procedures
- Developed a **regulatory communication plan** for two external stakeholders
- Created a full incident response flowchart

**Response Teams:**

| Team | Primary Role |
|:---|:---|
| Security Operations Center (SOC) | Continuous monitoring, triage, alert generation, documentation |
| Incident Response Team (IRT) | Decision making, regulatory compliance, stakeholder communications |
| IT & Identity Management Team | Credential management, access control, MFA enforcement, recovery |

**NIST IR Phases Covered:**

1. **Preparation** — detection tools, response team setup, legal frameworks, training and testing
2. **Detection & Analysis** — initial detection, threat classification, scope assessment, evidence collection
3. **Containment** — attack blocking, system isolation, data protection, operations continuity
4. **Eradication & Recovery** — vulnerability remediation, system hardening, data integrity restoration
5. **Post-Incident** — root cause analysis, regulatory reporting, security program improvement

**Tools Specified:**

| Tool | Purpose |
|:---|:---|
| Splunk Enterprise Security | SIEM — log correlation and suspicious pattern detection |
| CrowdStrike Falcon | EDR — endpoint monitoring and credential theft detection |
| Cisco Email Security Appliance | Email gateway — phishing detection and quarantine |
| KnowBe4 | Security awareness training and phishing simulations |
| RSA SecurID | MFA for executives and privileged users |

**Regulatory Communication Plan:**
- Central Bank of Barbados — 72-hour breach notification via encrypted email and registered mail
- TTSEC — formal regulatory portal filing with telephone follow-up

📄 [View Full Report](https://github.com/[Your-GitHub]/Incident-Response-Playbook)

* * *

## Professional Experience

* * *

### Junior Network Administrator
**Barbados Transport Board** &nbsp;|&nbsp; Bridgetown, Barbados &nbsp;|&nbsp; January 2025 – April 2025

**Responsibilities:**
- Configured and maintained network systems supporting daily operations across the organisation
- Troubleshot and resolved technical issues with bus driver tablets ensuring minimal downtime
- Provided hardware and software user support to staff across all departments
- Registered bus passes including student information ensuring data accuracy
- Updated and maintained electronic systems and devices across the organisation
- Delivered public speaking presentations and communications within the role

**Achievement:**

> Successfully set up the **GoCity Card system** — integrated student information into a secure database and connected it with bus driver tablets and card readers installed across buses throughout Barbados. This reduced manual processing, improved data accuracy, and ensured seamless fare collection across the network.

* * *

## Education

| Degree | Institution | Period |
|:---|:---|:---|
| BSc Computer Science & Electronic Engineering | University of the West Indies | 2025 – Present |
| Associate Degree in Applied Science – Computer Studies (GPA: 3.34) | Barbados Community College | 2023 – 2025 |
| Caribbean Examinations Council (CSEC) – General | The St. Michael Secondary School | 2018 – 2022 |

**Relevant Coursework — UWI:**
Computing 1, Computing 2, Unix, Digital Electronics, Digital Electronics 2, Introduction to Electronics, Basic Circuit Analysis

**Relevant Coursework — BCC:**
Webpage Design, Computer Concepts, Object-Oriented Programming & Design, Database Management Systems, Program Implementation using Java, System Analysis & Design, Application Development

* * *

## Connect With Me

- 📧 Email: [shakirwilliams07@gmail.com](mailto:shakirwilliams07@gmail.com)
- 🔗 LinkedIn: [linkedin.com/in/[Your-LinkedIn]](https://linkedin.com/in/[Your-LinkedIn])
- 💻 GitHub: [github.com/[Your-GitHub]](https://github.com/[Your-GitHub])

* * *

*"Security is not a product, but a process."* – Bruce Schneier
