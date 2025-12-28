---
title: "Hardening Edge Infrastructure: pfSense & VLAN Segmentation"
date: 2025-12-27
description: "Configuring a secure lab environment for offensive research."
tags: ["networking", "pfsense", "homelab"]
categories: ["Infrastructure"]
image: "cover.webp"
---

### Infrastructure Layout
To maintain OPSEC and isolate exploit testing, I’ve implemented a multi-VLAN structure.

* **VLAN 10 (Management):** Isolated for primary workstations.
* **VLAN 20 (Lab):** Where the "vulnerable" targets live.
* **VLAN 30 (Red):** Dedicated for C2 traffic and egress testing.

### Firewall Rules
Rules are configured on a **Deny-by-Default** basis. Only specific ports are mirrored to the IDS for traffic analysis.