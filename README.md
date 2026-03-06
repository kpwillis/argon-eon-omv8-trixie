# Argon EON NAS with OpenMediaVault 8 on Raspberry Pi OS Trixie

## Overview
This guide documents my experience running **OpenMediaVault 8** on
**Raspberry Pi OS Lite (Trixie)** using a **Raspberry Pi 4 (4 GB)** inside
an **Argon EON NAS case**.

---

## Hardware
- Raspberry Pi 4 (4 GB RAM)
- Argon EON NAS case
- Drives: (list yours)
- Power supply

## Software
- Raspberry Pi OS Lite (Trixie)
- OpenMediaVault 8
- Linux kernel: (optional)
- Tailscale
- Argon EON fan + LCD scripts

---

## Installation Order (Important)
1. Install Raspberry Pi OS Lite (Trixie)
2. Update system
3. Enable I2C
4. Install OpenMediaVault 8
5. Configure OMV storage
6. Install Tailscale
7. Install Argon EON scripts

---

## System Prep
```bash
sudo apt update
sudo apt full-upgrade -y
sudo reboot
