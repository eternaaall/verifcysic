# 🚀 Cysic Verifier Auto-Installer

This repository provides a one-command installation and management script for running Cysic Verifier nodes on GPU servers.

Created by **@eternaaall** 🧠

---

## 🔧 Features

- One-line install
- Interactive CLI menu
- Multi-session management via `screen`
- Per-session logs with tailing
- Auto-restart on failure
- Update + cleanup logic built-in

---

## 📦 Quick Start (1 Command Install)

```bash
bash <(curl -s https://raw.githubusercontent.com/eternaall/verifycysic/main/verifcys_byetrnl)
```

You will be prompted to enter your EVM wallet address on the first run.

---

## 📋 Menu Features

When running, the script presents a menu:

1. **View logs** of a specific screen session
2. **Start a new verifier session** (each in its own `screen`)
3. **Update verifier** (stops all, clears logs, reinstalls)
4. **Stop all sessions** and remove logs
5. **Exit** the manager

---

## 📂 Log Storage
- Logs are stored in `/var/log/cysic*.log`
- Each session has its own file: `cysic.log`, `cysic1.log`, etc.
- Logs auto-delete when sessions are stopped via menu
- Sessions auto-restart on failure

---

## ⚙️ Requirements

The script installs:
- `screen`
- `curl`

It automatically skips installation if already done.

---

## 🛡 License
MIT — Free to use and modify.

---

> ⭐ Found it useful? Consider giving the repo a star!
