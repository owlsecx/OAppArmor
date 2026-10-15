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

Offline AppArmor profile auditor & hardening advisor

---

## ✨ Features

- Tolerant AppArmor policy parser — profiles, hats, child profiles, flags, include / include if exists, abi, alias, variables (@{VAR}), conditionals, and every rule class: file, capability, network, mount, remount, umount, pivot_root, ptrace, signal, dbus, unix, change_profile, rlimit, userns, io_uring, mqueue
- Offline scan of /etc/apparmor.d under any --root (mounted images, backups, container rootfs)
- Variable expansion from tunables/ with sane defaults
- AppArmor-glob → regex engine with deny-precedence evaluation of sensitive targets (/proc/*/mem, shadow…)
- 45+ detection rules mapped to CWE + MITRE ATT&CK with severity, rationale and concrete remediation
- Disabled (disable/) and force-complain detection
- High-risk binary coverage check (known list)
- Per-profile score + overall A+…F grade
- Reports: TXT / Markdown / JSON / CSV / SARIF 2.1.0
- CI gate: --fail-on SEVERITY, --min-severity filter
- --demo self-test with synthetic weak/hardened tree
- Read-only by design — never modifies policy

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OAppArmor
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
