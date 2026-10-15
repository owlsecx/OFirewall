# 🦉 OFirewall

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-ONetwork-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OFirewall** — Offline Firewall Ruleset Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

Offline firewall ruleset auditor (iptables / nftables / ufw / firewalld)

---

## ✨ Features

- Tolerant parsers for iptables-save / ip6tables-save, nft list ruleset (incl. named sets), ufw (user.rules, /etc/default/ufw, ufw.conf, `ufw status verbose`) and firewalld (zone XML, firewalld.conf, --list-all)
- Format auto-detection and directory scanning
- Normalised rule model (proto / addr / port / iface / conntrack state / verdict) for cross-framework checks
- ANY/ANY accept and exposed admin-port detection (SSH, RDP, VNC, DB, Docker, k8s, SMB, SNMP ...)
- Shadowed / redundant / conflicting rule analysis using rule-space subsumption & overlap logic
- Default-policy, missing-logging, ordering, loopback, conntrack, ICMP/ICMPv6, IPv6-parity, NAT checks
- Weighted A+…F grade with per-category subscores
- Hardening suggestions with CIS / NIST references
- Exports: TXT / Markdown / JSON / CSV / SARIF 2.1.0
- Optional read-only live capture (iptables-save, nft list ruleset) — never modifies the firewall
- Built-in insecure demo rulesets for self-test
- Full CLI mode (--path, --fail-on, --min-severity ...)

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OFirewall
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
