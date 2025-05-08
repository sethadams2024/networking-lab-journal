# 🖥️ Lenovo Lab PC Setup (Donated System)

This system was donated by a family friend. It’s now part of my IT and networking home lab for experimentation and learning.

---

## 🛠️ Initial System Setup

- **Initial Specs**:
  - **CPU**: AMD A10-7800 with integrated graphics
  - **Motherboard**: Lenovo Bantry CRB (PCIe 3.0, 8.0GT/s)
  - **Memory**: 1 × 12GB DDR3 1600MHz + 1 × 4GB DDR3 1600MHz (Total: 16GB)
  - **Storage**: HDD (planned upgrade to SSD)
  - **GPU**: None (using integrated graphics from APU)

- **Initial Actions**:
  - System reset stuck at 22%; forced shutdown and restarted successfully.
  - Forgot to disconnect Wi-Fi during setup (unable to bypass Microsoft login).
  - Configured with local admin account and limited Microsoft telemetry.
  - Created two standard users (`User1111`, `User2222`) for testing purposes.
  - Performed full system updates post-installation.

---

## 🔧 Tools & Software Installed

- **CPU-Z**:
  - Installed and used to inspect CPU, RAM, and motherboard specs.

---

## 🛠️ Planned Hardware Upgrades

- ✅ **Install SSD** (to replace current slow HDD)
  - Will clone OS and reconfigure boot settings in UEFI.
- 🧠 **Upgrade RAM** (prefer matched modules for dual-channel performance)
- ❄️ **Replace CPU Fan** (optional; if thermal issues arise during load testing)

---

## 👤 User Management Setup

Steps followed:

1. Opened `Settings → Accounts → Family & Other Users`
2. Created:
   - Admin account (my own)
   - Two local standard accounts:
     - `User1111`
     - `User2222`
3. Skipped Microsoft account linking for all users.

---

## 🔐 Remote IT Role-Based Access

Testing user roles and local administrative separation.  
➡️ [View Role Access Setup](./roleaccess.md)

---

## 🧪 Learning Objectives

- Practice cloning and migrating OS to SSD  
- Explore BIOS/UEFI configuration and boot management  
- Test account permissions and local user administration  
- Simulate real-world IT support tasks (e.g., user lockouts, password resets)  
- Document and manage tasks using my osTicket-based ticketing system  

