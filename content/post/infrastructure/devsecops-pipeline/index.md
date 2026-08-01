---
title: "DevSecOps CI/CD Security Pipeline"
date: 2026-08-01
draft: false
tags: ["DevSecOps", "GitHub Actions", "Trivy", "Semgrep", "OWASP ZAP", "Docker"]
categories: ["infrastructure"]
description: "A Secure SDLC pipeline integrating SAST, DAST, secrets scanning, and container scanning — gates reject builds on critical CVEs."
---

> 🚧 **Full write-up coming soon.** Architecture, pipeline YAML, and scan result examples are being documented.

## Overview

A production-ready Secure SDLC pipeline that integrates four scanning layers into a GitHub Actions workflow. Build gates reject automatically when critical CVEs or exposed credentials are detected.

## Pipeline Stages

| Stage | Tool | Purpose |
|-------|------|---------|
| SAST | Semgrep | Static code analysis |
| Secrets Scanning | truffleHog | Credential leak detection |
| Container Scanning | Trivy | Image CVE analysis |
| DAST | OWASP ZAP | Dynamic runtime scanning |

## Stack

`Python` `GitHub Actions` `Trivy` `Semgrep` `OWASP ZAP` `truffleHog` `Docker`

## Status

- [x] Pipeline engineered and functional
- [x] Severity triage and build gates configured
- [ ] Full write-up and YAML reference in progress
