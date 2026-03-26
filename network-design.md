---
layout: default
---

# Enterprise Network Design
### Cybersecurity Bootcamp Capstone &nbsp;|&nbsp; September 2025

[Back to Portfolio](./index.html)

* * *

## Objective

Design and build a full secure enterprise network topology for a banking organisation from scratch using Cisco Packet Tracer — meeting banking-grade security requirements including PCI DSS compliance.

* * *

## What I Did

I designed the entire network architecture, configured all devices, wrote firewall rules, and documented the security theory behind every design decision.

* * *

## Network Architecture

| VLAN | Department | Subnet |
|:---|:---|:---|
| VLAN 10 | Management | 192.168.10.0/24 |
| VLAN 20 | Finance | 192.168.20.0/24 |
| VLAN 30 | Public Relations | 192.168.30.0/24 |
| VLAN 40 | IT Department | 192.168.40.0/24 |
| VLAN 50 | R&D | 192.168.50.0/24 |
| VLAN 60 | Guest Network | 192.168.60.0/24 |
| VLAN 100 | Infrastructure Servers | 192.168.100.0/24 |
| VLAN 110 | PCI DSS Payment Database | 192.168.110.0/24 |
| VLAN 120 | PII Customer Database | 192.168.120.0/24 |

* * *

## Infrastructure Configured

**Servers:**
- DHCP Server — 192.168.100.11
- DNS Server — 192.168.100.10
- Mail Server — 192.168.100.12
- Application Server — 192.168.100.13

**Banking Database Servers:**
- PCI DSS Database — 192.168.110.10
- PII Database — 192.168.120.10
- Hardware Security Module (HSM)
- Database Monitor

**Network Devices:**
- Multilayer Switch 1 (Cisco 3560-24PS) — core switching and inter-VLAN routing
- Multilayer Switch 2 — secondary switching
- Dual Cisco 2811 Routers — redundancy and ISP connections
- Cisco ASA 5506-X Firewall — perimeter security

* * *

## Firewall Rules Written

| Rule | Action | Purpose |
|:---|:---|:---|
| Rule 1 | DENY | Block external access to database ports — SQL Server 1433, MySQL 3306, PostgreSQL 5432 |
| Rule 2 | PERMIT | Allow management VLAN HTTPS access during business hours only (8AM–6PM) |
| Rule 3 | DENY | Block guest network from accessing PCI DSS and PII databases |
| Rule 4 | PERMIT | Allow Finance VLAN secure HTTPS access to payment systems only |
| Rule 5 | PERMIT | Force all outbound traffic through proxy for content filtering and malware scanning |

* * *

## Security Theory Documented

**Maintaining Availability**
Implemented Hot Standby Router Protocol (HSRP) for automatic failover, dual ISP connections with BGP routing, N+1 clustered banking servers with real-time data replication, and Spanning Tree Protocol Rapid-PVST+ for 50ms convergence during link failures.

**Protecting Sensitive Data**
PCI DSS database encrypted with AES-256. Encryption keys managed by Hardware Security Module. Data in transit protected by TLS 1.3 with perfect forward secrecy. PII database uses data tokenisation so stolen tokens cannot reveal real customer information.

**Secure Inter-Departmental Communication**
Layer 3 switches route inter-VLAN traffic at full speed using ASICs. Trunk links carry multiple VLAN traffic simultaneously using IEEE 802.1Q tagging. MACsec encrypts traffic between switches. VoIP calls protected by SRTP and TLS.

**Limiting Attack Surface on Public-Facing Systems**
All customer-facing banking services hosted in a hardened DMZ. Web Application Firewall blocks SQL injection, XSS, and DDoS attacks in real time. NGINX reverse proxy hides internal network structure. Geographic IP filtering restricts traffic from high-risk regions.

* * *

## Key Takeaway

Network segmentation through VLANs and strict ACL rules is one of the most effective ways to limit the blast radius of a breach. Even if an attacker compromises one segment, proper segmentation prevents lateral movement to critical systems.

* * *

[Back to Portfolio](./index.html)
