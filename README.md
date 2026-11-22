# 🦉 OAppArmor

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OScan-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OAppArmor** — Offline AppArmor Profile Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OAppArmor is an offline, read-only auditor for AppArmor confinement policy that never modifies the profiles it reads. Its tolerant parser understands profiles, hats, child profiles, flags, includes, variables and every rule class, and it can evaluate a live system or any mounted image, backup or container rootfs via --root. More than 45 detection rules are mapped to CWE and MITRE ATT&CK with per-profile scoring and an overall A+…F grade.

---

## ✨ Features

- Tolerant parser for profiles, hats, child profiles, includes, variables and all rule classes
- Offline scanning of /etc/apparmor.d under any --root (images, backups, rootfs)
- AppArmor-glob → regex engine with deny-precedence on sensitive targets
- 45+ rules mapped to CWE + MITRE ATT&CK with severity and remediation
- High-risk binary coverage checks and complain/disabled-profile detection
- Per-profile score, A+…F grade and export to TXT/MD/JSON/CSV/SARIF 2.1.0

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OAppArmor --scan
./OAppArmor --profile /etc/apparmor.d/usr.sbin.nginx --format json
./OAppArmor --root /mnt/image --scan --fail-on high
./OAppArmor --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 275+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled.s.Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
