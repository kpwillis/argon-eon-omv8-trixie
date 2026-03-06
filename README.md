# Argon EON NAS with OpenMediaVault 8 on Raspberry Pi OS Trixie

## Overview
This guide documents my experience running **OpenMediaVault 8** on
**Raspberry Pi OS Lite (Trixie)** using a **Raspberry Pi 4 (4 GB)** inside
an **Argon EON Pi NAS**.  I have older equipment lying around not being utilized.
After days of frustration I found this easiest method to getting the
equipment up and running.

---

## Hardware
- Raspberry Pi 4 (4 GB RAM)
- Argon EON Pi NAS
- Drives: (list yours)
- Power supply

## Software
- Raspberry Pi OS Lite (Trixie)
- Argon EON fan + LCD scripts
- OpenMediaVault 8
- Tailscale

---

## Installation Order (Important)
1. Install Raspberry Pi OS Lite (Trixie)
2. Update system
3. Enable I2C
4. Install Argon EON scripts
5. Install OpenMediaVault 8
6. Configure OMV storage
7. Install Tailscale

---

## System Prep
```bash
sudo apt update
sudo apt full-upgrade -y
sudo reboot

