---
title: "Resume"
url: "/page/resume/"
description: "mohamed@meddah.systems"
---

📄 [Download PDF version](https://meddah.systems/cv)

---

## Mohamed MEDDAH

**Cybersecurity Engineer | Cloud Security | Offensive Security**

📍 Marrakech, Morocco · 🌍 Open to relocation · Open to remote
📧 mohamed@meddah.systems · [linkedin.com/in/meddah](https://linkedin.com/in/meddah) · [github.com/mrmeddah](https://github.com/mrmeddah) · [meddah.systems](https://meddah.systems)

---

## 🎯 Professional Summary

Final-year Cybersecurity Engineering student (Bac+5 / Master's equivalent, Bologna Process EQF Level 7, expected Jun. 2027) with confirmed production bug bounty impact and cloud security tooling across Azure and AWS. Proven across offensive web and API testing, Azure RBAC privilege escalation research, and DORA-aligned defensive tooling. Proficient in English (C1) and French (B2). Seeking PFE internship in EU regulated environments from February 2027.

---

## 🛠️ Technical Skills

**Offensive Security:** Penetration Testing, Web Application Security, API Security, SSRF, IDOR/BOLA, OAuth 2.0 Exploitation, GraphQL Security, Subdomain Enumeration, AD Attacks, NTLM Relay, ADCS Abuse, LFI

**Cloud Security — Azure:** Security Posture Management, Defender for Cloud, Microsoft Entra ID, Conditional Access, Managed Identities, Azure RBAC, Key Vault, Azure Functions, ARM Templates, Azure Monitor

**Cloud Security — AWS:** EC2, VPC, IAM, S3, RDS, Secrets Manager, CloudTrail, Security Hub, GuardDuty, 70+ services via Terraform IaC

**Frameworks & Standards:** OWASP Top 10, OWASP API Security Top 10, MITRE ATT&CK, CWE, Zero Trust, DORA, NIS2, ISO 27001

**Network:** TCP/IP, BGP, OSPF, VXLAN/EVPN, VLANs, pfSense, Site-to-Site VPN, GNS3, Wireshark (CCNA/CCNP level)

**Security Tools:** Burp Suite Professional, Nmap, Subfinder, Amass, httpx, Feroxbuster, ffuf, Shodan, truffleHog, BloodHound, Metasploit

**Development:** Python, Bash, JavaScript, Java, Go, C++, Django, React, Node.js

**Systems:** Linux (Debian/Ubuntu/Kali), Windows Server, Active Directory, Docker

---

## 💼 Professional Experience

### Independent Contractor — Data Curator
**Veeva Systems** · Remote · Mar. 2024 – Sep. 2024

- Processed and validated large-scale structured datasets for pharmaceutical CRM pipelines; maintained data integrity and compliance standards across a multi-client regulated environment, directly applicable to NIS2/DORA data governance requirements.

### IT Infrastructure Intern
**Menara Prefa** · Marrakech, Morocco · April 2024

- Deployed and configured pfSense firewall (packet filtering, NAT, segmentation); implemented site-to-site VPN using IPsec tunnelling.

### Development & Systems Administration Intern
**Municipality of El Kelaa des Sraghna** · El Kelaa, Morocco · August 2023

- Built full-stack citizen ticket management application integrated with the national Chikaya platform; RBAC-based routing; Django REST / React / relational DB; Windows Server and Linux administration.

---

## 🏗️ Projects

### Azure RBAC Privilege Escalation Mapper
*Python | Azure SDK | Microsoft Graph API | Azure Functions · September 2026*

- Enumerates multi-hop Azure privilege escalation paths via RBAC misconfiguration; detects the runCommand/IMDS token theft chain — a Defender for Cloud blind spot.
- Maps four attack primitives: Run Command abuse, Custom Script Extension backdoor, Role Assignment write escalation, User Data injection; outputs attacker-ready PoC commands with inline DORA Article 9 and CSSF regulatory citations.

### Azure Deployment History Sanitizer
*Python | Azure Functions | ARM API | Shannon Entropy Analysis · July 2026*

- Serverless tool purging ARM/Bicep deployment histories that expose plaintext secrets to any Reader-level account; Shannon entropy + keyword heuristics detect credentials, SAS tokens, and connection strings.
- Three modes: aggressive purge, selective entropy-based, and audit-only; full audit trail to Azure Storage Tables for DORA compliance and CSSF audit readiness.

### Zero-Trust Distributed Storage System
*Go | Java | libsodium | AES-256-GCM | ABE | JWT · May 2026*

- Mini-IPFS with client-side AES-256-GCM encryption (libsodium), Merkle DAG integrity, 3-node replication, and cryptographic access control via Attribute-Based Encryption and Proxy Re-Encryption; JWT Ed25519 PoP tokens with nonce-based anti-replay (TTL 30s).

### AWS Cloud Infrastructure (Terraform IaC)
*Terraform | AWS | IAM | VPC | Secrets Manager · Feb. 2025*

- Provisioned 70+ AWS services via modular Terraform on a live account: least-privilege IAM policies, Secrets Manager integration, multi-service network architecture across EC2, RDS, VPC, S3, and 60+ additional services.

### EVPN/VXLAN Spine-Leaf Datacenter Fabric
*FRRouting | GNS3 | BGP EVPN | Linux iproute2 · 2026*

- Deployed EVPN/VXLAN overlay on GNS3 with FRRouting (BGP EVPN, OSPF underlay), Route Reflector, and MP-BGP L2VPN; validated MAC/IP distribution via Wireshark; identified VXLAN attack surface: BGP EVPN route poisoning and frame injection via underlay access.

---

## 🐛 Bug Bounty & Security Research

**Active Researcher — HackerOne | Intigriti | Bugcrowd** (public and private programs) · Mar. 2024 – Present

| Severity | Finding |
|----------|---------|
| **Critical (CVSS 9.1)** | Unauthenticated account creation chained with Django DEBUG mode leaking cloud credentials and JWT secrets, then BOLA/IDOR to full attendee PII exfiltration (CWE-200, CWE-284) |
| **High — OAuth ATO** | redirect_uri validation bypass on GitLab SSO flow — 1-click account takeover on an artifact repository via authorization code grant misconfiguration |
| **High — SSRF** | Host Header auth bypass on a global advertising platform; reached live Kubernetes microservice returning production data (CWE-918) |
| **Medium — Info Disclosure** | Exposed Swagger UI, Spring Boot Actuator, internal IP leakage on enterprise IoT/B2B SaaS; extracted API constants from obfuscated JS bundles |
| **Medium — Credential Exposure** | Unauthenticated AI API keys, search credentials, and internal endpoints live on global e-commerce infrastructure (CWE-548) |
| **Medium — Admin Exposure** | JBoss/WildFly admin console on telecoms infrastructure; AD FS and WS-Trust endpoint enumeration with timing analysis |

**Methodology:** Subfinder, Amass, httpx, Shodan, Feroxbuster, ffuf, gau, Katana, truffleHog, Burp Suite Professional; OWASP Top 10, OWASP API Security Top 10, CWE classification.

---

## 🏁 CTF & Labs

- **SecDojo National CTF:** Ranked #100 / 3,500+ participants — top 3% nationally. Techniques: LSASS credential dump, BloodHound attack paths, ADCS ESC11, NTLM relay.
- **MCP/Prompt Injection Lab (NebulaAssist):** Full attack chain — Nmap recon, SSE token extraction, hidden tool enumeration via prompt injection.

---

## 🎓 Education

| Period | Degree | Institution |
|--------|--------|-------------|
| 2024 – Jun. 2027 (expected) | State Engineer's Degree in Cybersecurity & Network Infrastructure — Bac+5 / EQF Level 7 | EMSI — École Marocaine des Sciences de l'Ingénieur, Marrakech |
| 2022 – 2024 | Specialized Technician Diploma — Network & Systems Administration | ISTA — Institut Spécialisé de Technologie Appliquée (OFPPT), Marrakech |

---

## 📜 Certifications

| Certification | Issuer | Date |
|---------------|--------|------|
| AWS Certified Cloud Practitioner (CLF-C02) | Amazon Web Services | Jul. 2026 |
| Microsoft Certified: Cloud & AI Security Engineer Associate (SC-500) | Microsoft | Sep. 2026 |
| AWS Certified Solutions Architect — Associate (SAA-C03) | Amazon Web Services | Oct. 2026 |

---

## 🌍 Languages

| Language | Level |
|----------|-------|
| Arabic | Native |
| French | Professional proficiency (CEFR B2) |
| English | Professional proficiency (CEFR C1) |
