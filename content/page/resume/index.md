---
title: "Resume"
layout: "page"
---

## 🧑‍💻 MEDDAH Mohamed

**Cybersecurity & Network Infrastructure Engineer**

📍 Marrakech, Morocco · 🌍 Open to international mobility
📧 mrmeddah@yahoo.com
🔗 [linkedin.com/in/meddah](https://linkedin.com/in/meddah) · [github.com/mrmeddah](https://github.com/mrmeddah) · [meddah.systems](https://meddah.systems)

---

## 🎯 Profile

Final-year cybersecurity engineering student (Bac+5), specialized in **offensive security**, **network infrastructure**, and **cloud security**. Active bug bounty hunter on HackerOne, Intigriti, and Bugcrowd with confirmed findings on production targets. Deployed 70+ AWS services via Terraform on a real account; built a Zero-Trust storage system from scratch.

---

## 🎓 Education

| Period | Degree | Institution |
|--------|--------|-------------|
| 2024 – 2027 | **State Engineer in Cybersecurity & Network Infrastructure** (Bac+5) | EMSI — École Marocaine des Sciences de l'Ingénieur, Marrakech |
| 2022 – 2024 | **Specialized Technician — Network & Systems Administration** | ISTA — OFPPT, Marrakech |

---

## 💼 Experience

### Freelance Contractor — Data Curator
**Veeva Systems** · Remote · Mar – Sep 2024

- Processing and validation of large-scale structured datasets for pharmaceutical CRM pipelines
- Maintained data integrity and compliance standards in a multi-client environment

### IT Infrastructure Intern
**Menara Prefa** · Marrakech · Apr 2024

- Deployed and configured a pfSense firewall: filtering rules, NAT, network segmentation, traffic monitoring
- Set up a site-to-site VPN for inter-site corporate connectivity

### Development & Systems Administration Intern
**Municipality El Kelaa des Sraghna** · 2023

- Built a full-stack citizen ticket management app integrated with the national Chikaya platform, with automatic routing to relevant departments
- **Stack:** Django (REST backend), React (frontend), relational database
- Windows Server and Linux systems administration and network diagnostics

---

## 🏗️ Projects

### 🔒 Zero-Trust Distributed Storage System
[github.com/mrmeddah](https://github.com/mrmeddah) · May 2026

- Mini-IPFS with AES-256-GCM client-side encryption (libsodium), Merkle DAG integrity verification, 3-node replication
- Zero-Trust auth: JWT Ed25519 Proof-of-Possession, stateless tokens scoped per operation and CID, nonce anti-replay (30s TTL)
- Cryptographic access control via ABE (Attribute-Based Encryption) & Proxy Re-Encryption — no master key exposure
- 6 security objectives validated (PASS): passive eavesdropping, tampering, node collusion
- **Stack:** Go, Java Sockets, libsodium, SHA-256, X25519/ECDH

### 🌐 EVPN/VXLAN Fabric — Modern Datacenter VPN
[github.com/mrmeddah](https://github.com/mrmeddah) · 2026

- EVPN/VXLAN Spine-Leaf overlay on GNS3 with Linux nodes and FRRouting (BGP EVPN, OSPF underlay)
- VTEP config, Route Reflector, MP-BGP L2VPN EVPN, Linux bridge/VXLAN datapath; Wireshark validation
- Attack surface identification: no native encryption, BGP EVPN poisoning, frame injection vectors
- **Stack:** FRRouting, GNS3, Linux iproute2, Wireshark, BGP/OSPF

### ☁️ AWS Cloud Infrastructure — Terraform
Personal project

- Provisioned 70+ AWS services via modular Terraform on a real account (RDS, EC2, VPC, IAM, Secrets Manager, S3…)
- Least-privilege IAM policies, Secrets Manager integration, multi-service network architecture

### 💬 ChainTalk B2B — Web2.5 Blockchain Chat
Personal project

- Real-time messaging app with blockchain integration
- **Stack:** React 18, Vite, TailwindCSS, Ethers.js, Node.js, Express, Socket.io, PostgreSQL, Solidity, Hardhat

---

## 🐛 Bug Bounty & Security Research

Active hunter on **HackerOne**, **Intigriti**, **Bugcrowd** (public & private programs)

| Target | Platform | Finding |
|--------|----------|---------|
| **Yahoo** | Intigriti | Unauthenticated internal SSRF via Host Header auth bypass on Prebid Server; accessed internal Kubernetes microservice `goldfinger--staging-use1:4080` with real ad data (CWE-918) |
| **SFS Group** | Intigriti · High | OAuth `redirect_uri` validation bypass on GitLab SSO → 1-click Account Takeover on JFrog Artifactory |
| **SFS Group** | Intigriti · Critical 9.1 | Chain: unauth account creation → Django DEBUG in prod (leaked AWS keys, PostgreSQL creds, JWT) → platform-wide BOLA → attendee PII exfiltration (CWE-200 / CWE-284) |
| **T-Mobile / USCellular** | Bugcrowd | Exposed Swagger UI, Spring Boot Actuator endpoints, internal IP leakage — Nokia WING/JHipster stack |
| **Vodafone Oman** | Intigriti | Exposed WildFly/JBoss admin interface; API constants extracted from React B2B JS bundle; AD FS / WS-Trust analysis |
| **Verisign** | Bugcrowd | MCP server exposure, tunnel endpoints, subdomain leakage via CSP |
| **Watsons / AS Watson** | Intigriti | Unauthenticated credential exposure — AI API key, Algolia key, internal endpoints (CWE-548) |
| **Whatnot** | HackerOne | GraphQL authorization testing and IDOR |

**Toolbox:** subfinder, amass, httpx, Shodan, feroxbuster, ffuf, gau, katana, truffleHog, Burp Suite

---

## 🏁 CTF & Labs

- **CTF National SecDojo** — Ranked #100 / 3,500+ participants; all challenges solved except one AD scenario
- **Active Directory Lab (AD105)** — Multi-forest, LSASS dump, BloodHound, ADCS ESC11, NTLM relay, hash extraction
- **MCP/Prompt Injection Lab (NebulaAssist)** — Full chain: nmap → SSE token extraction → hidden tool enumeration
- **Unicode Steganography CTF** — Solved

---

## 🖥️ Virtualization & Monitoring

### Hypervisors
- VMware ESXi & Proxmox VE: VM deployment, resource management, snapshots, migration
- GNS3 with VM integration for complex network topologies (OSPF, BGP, VXLAN/EVPN)
- Packet Tracer for Cisco network config validation

### Monitoring & Observability
- **Zabbix**: router & switch supervision, SNMP MIB performance metrics on Linux
- **Grafana**: custom SOC dashboard — real-time network performance (CPU, bandwidth, interface availability)
- **Splunk**: log ingestion and security event correlation
- **pfSense**: network monitoring, traffic filtering, firewall rules, intrusion alerts

---

## 🛠️ Technical Skills

| Domain | Skills |
|--------|--------|
| **Offensive Security** | Recon, enumeration, misconfigurations, LFI, server-side vulns, API security, GraphQL, AD attacks, NTLM relay, ADCS abuse |
| **Infrastructure** | TCP/IP, DNS, DHCP, VLANs, VPN, pfSense, OSPF, BGP, EVPN/VXLAN |
| **Cloud** | AWS (70+ services), Terraform, IAM, VPC, S3, RDS, Secrets Manager |
| **Development** | C++ (security tooling), Java, Python, Go, Bash, SQL, Django, React |
| **Virtualization** | VMware ESXi, Proxmox, GNS3, VirtualBox |
| **Monitoring** | Zabbix, Grafana, Splunk, pfSense |
| **Tools** | nmap, Wireshark, Metasploit, ffuf, hashcat, gdb, Burp Suite, BloodHound |

---

## 📜 Certifications

| Certificate | Issuer | Date |
|-------------|--------|------|
| Fundamentals of Blockchain Architecture | LearnQuest | Apr 2026 |
| Introduction to Cloud Computing | IBM | Nov 2025 |
| Introduction to NoSQL Databases | IBM | Dec 2025 |
| Introduction to DevOps | IBM | Jan 2025 |
| Basics of Cisco Networking | LearnQuest | Dec 2024 |

---

## 🌍 Languages

| Language | Level |
|----------|-------|
| Arabic (Darija) | Native |
| French | Professional |
| English | Professional |

---

> *References and project documentation available on request.*
