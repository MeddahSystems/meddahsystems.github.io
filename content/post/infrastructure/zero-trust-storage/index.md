---
title: "Zero-Trust Distributed Storage System"
date: 2026-05-01
draft: false
tags: ["Cryptography", "Go", "Java", "Zero Trust", "libsodium", "ABE", "JWT"]
categories: ["infrastructure"]
description: "A mini-IPFS with AES-256-GCM encryption, Merkle DAG integrity, 3-node replication, and Attribute-Based Encryption access control."
---

> 🚧 **Full write-up coming soon.** This page is a placeholder — cryptographic architecture diagrams, code walkthroughs, and security validation results are being documented.

## Overview

A content-addressed distributed storage system built from first principles with a Zero Trust authentication layer. Every node is treated as untrusted; access is governed by cryptographic proofs, not network perimeter.

## Key Properties

| Property | Implementation |
|----------|----------------|
| Encryption | Client-side AES-256-GCM via libsodium |
| Integrity | Merkle DAG verification |
| Replication | 3-node with cryptographic consistency |
| Access Control | Attribute-Based Encryption + Proxy Re-Encryption |
| Authentication | JWT Ed25519 Proof-of-Possession |
| Anti-Replay | Nonce-based, TTL 30s |

## Stack

`Go` `Java` `libsodium` `AES-256-GCM` `Attribute-Based Encryption (ABE)` `JWT Ed25519`

## Status

- [x] System designed and implemented
- [x] Validated against 6 security objectives including node collusion resistance
- [ ] Full cryptographic write-up in progress
