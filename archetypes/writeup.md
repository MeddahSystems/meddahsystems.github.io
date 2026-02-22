---
title: '{{ replace .Name "-" " " | title }}'
description: 'A professional penetration testing write-up for the {{ replace .Name "-" " " | title }} machine.'
date: {{ .Date }}
image: "cover.webp"
categories:
    - Offensive
tags:
    - HackTheBox
    - Writeup
    - Boot2Root
draft: true
---

> **Note to self:** Drop a screenshot or logo of the machine into this post's folder and name it `cover.webp` so the Stack theme automatically uses it as the thumbnail!

## 1. Executive Summary

> *Write a brief paragraph summarizing the engagement. Focus on the business impact: how did you get in, how did you get root, and what is the overarching vulnerability type?*

The target server, **{{ replace .Name "-" " " | title }}**, was compromised due to [insert primary web/external vulnerability], leading to initial access as a low-privileged user. Privilege escalation to root was subsequently achieved by exploiting [insert internal misconfiguration/exploit]. 

---

## 2. Reconnaissance & Enumeration

### Nmap Scan Results

A full TCP port scan was conducted to identify externally facing services.

```bash
nmap -sC -sV -p- <TARGET_IP>

```

* **Port 22 (SSH):** [Version Info]
* **Port 80 (HTTP):** [Version Info]
* **Port [XXX] ([Service]):** [Version Info]

### Web Enumeration

> *Detail your directory brute-forcing (Gobuster/ffuf) or subdomain enumeration. Mention any interesting files, login pages, or exposed version numbers found.*

```bash
# Insert your Gobuster or FFUF command here

```

---

## 3. Initial Access / Vulnerability Exploitation

### The Vulnerability

> *Explain the flaw (e.g., Default credentials on the admin portal, SQL Injection, arbitrary file upload).*

### The Exploit

> *Explain the steps taken to weaponize the flaw. Did you upload a PHP reverse shell? Did you intercept traffic with Burp Suite?*

### The Payload

The following payload was used to establish a reverse shell connection back to the attacking machine:

```bash
# Insert your payload or exploit code here

```

---

## 4. Privilege Escalation

### Internal Enumeration

> *What specific misconfiguration stood out? (e.g., "Checking `sudo -l` revealed that the user could execute a specific script as root without a password," or "LinPEAS identified an outdated kernel version vulnerable to PwnKit.")*

### The Exploitation Path

> *Detail exactly how you abused that misconfiguration. Show the code/commands you used to elevate privileges.*

```bash
# Insert your PrivEsc commands here

```

Proof of root access:

```bash
# id
uid=0(root) gid=0(root) groups=0(root)

```

---

## 5. Remediation & Mitigation

> *This section separates you from standard CTF players. Tell the hypothetical client how to fix the holes you just exploited.*

* **Fixing Initial Access:** [e.g., Enforce strong password policies for the admin portal, implement strict input validation to prevent arbitrary file uploads, patch the Apache service to the latest stable release.]
* **Fixing Privilege Escalation:** [e.g., Remove the `NOPASSWD` directive in the `/etc/sudoers` file, enforce the principle of least privilege, update the Linux kernel.]

---

## 6. Key Takeaways

> *A brief, honest section about what you learned, what rabbit holes you fell into, or what troubleshooting you had to do.*

* Takeaway 1
* Takeaway 2

```

