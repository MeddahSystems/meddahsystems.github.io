---
title: "Adversary Simulation & Detection Engineering Lab"
date: 2026-08-01
draft: false
tags: ["Azure", "Sentinel", "KQL", "MITRE ATT&CK", "Terraform", "Red Team"]
categories: ["infrastructure"]
description: "5 end-to-end attack chains across 13 MITRE ATT&CK techniques with full KQL detection coverage in Microsoft Sentinel."
---

> 🚧 **Full write-up coming soon.** Detailed documentation, attack chain diagrams, and detection rule breakdowns are being written up.

## Overview

This lab executes 5 complete adversarial attack chains across 13 MITRE ATT&CK techniques, with each attack paired with engineered KQL detection rules in Microsoft Sentinel and a coverage gap analysis.

## Attack Chains

| Chain | Technique | ATT&CK ID |
|-------|-----------|-----------|
| Phishing-to-Domain Compromise | Spearphishing, Credential Dumping | T1566, T1003 |
| Entra ID Identity Attacks | Pass-the-PRT, Token Theft | T1528, T1550 |
| Cloud Misconfiguration Exfil | Abuse Elevation Control Mechanism | T1548 |
| On-Prem to Cloud Lateral Movement | PRT Abuse via AADInternals | T1550.001 |
| Backdoor Service Principal | Persistence via Application | T1098.001 |

## Stack

`Azure` `Terraform` `Microsoft Sentinel` `KQL` `Containerlab` `Sysmon` `Mimikatz` `Impacket` `AADInternals` `ROADtools` `Python` `PowerShell`

## Status

- [x] Attack chains designed and executed
- [x] KQL detection rules written
- [x] Coverage gap analysis completed
- [ ] Full write-up in progress
