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

## 🔐 Role-Based Access

Testing user roles and local administrative separation.  
➡️ [View Role Access Setup](./roleaccess.md)

---

## 🧪 Learning Objectives

- Practice cloning and migrating OS to SSD  
- Explore BIOS/UEFI configuration and boot management  
- Test account permissions and local user administration  
- Simulate real-world IT support tasks (e.g., user lockouts, password resets)  
- Document and manage tasks using my osTicket-based ticketing system  


------------------------------------------------------------------------------------
<br>
<br>
<br>









# Lenovo H50 Upgrade: PSU and GPU Installation Summary

## 🖥️ Original System Specs
- **Model:** Lenovo H50-55
- **CPU:** AMD A10-7800 APU with integrated Radeon R7 Graphics
- **Motherboard:** OEM Lenovo microATX
- **Original PSU:** ~280W proprietary PSU (non-standard connectors)
- **Case Type:** OEM tower (tight clearance, limited airflow)

---

## ⚙️ Upgrade Components

### 🔌 Power Supply
- **Model:** Helios 650W ATX PSU
- **Connectors Used:**
  - 24-pin ATX (main board power)
  - 4-pin CPU power (from EPS split cable)
  - 6-pin PCIe (for GPU)
- **Modular:** No
- **Testing:**
  - ✅ Passed paperclip test (PSU fan spins)
  - 🔁 Reset CMOS using "CLR_CMOS SW" and jumper

### 🎮 Graphics Card
- **Model:** NVIDIA GeForce RTX 1650 (single fan)
- **Power Connector:** 6-pin PCIe
- **Display Outputs:** HDMI, DVI-D, DisplayPort

---

## 🛠️ Installation Summary

### 1. **Removed Original PSU**
- Detached 24-pin and 4-pin motherboard connectors
- Removed old PSU from case

### 2. **Installed Helios 650W PSU**
- Connected:
  - 24-pin ATX to motherboard
  - 4-pin CPU (from EPS12V split)
  - 6-pin PCIe to GPU
- Verified PSU switch was set to "I" (on)

### 3. **Installed RTX 1650 GPU**
- Inserted into PCIe x16 slot
- Noticed plastic tab in slot (normal retention clip)
- Connected 6-pin PCIe power

### 4. **First Boot**
- System powered on, but **no display output**
- Moved display cable from motherboard to GPU ✅
- Performed **CMOS reset** using:
  - "CLR_CMOS SW" button
  - Later attempted jumper reset

---

## 🧪 Diagnostics and Troubleshooting

### ✅ PSU Verified Working
- Fan spun during paperclip test
- Powered motherboard and fans

### ⚠️ GPU No Display Initially
- Confirmed monitor connected to GPU (not motherboard)
- No beeps or display from POST
- Suspected:
  - BIOS auto-switching issue
  - CMOS/BIOS stuck settings
  - Possibly incompatible GPU initialization

### 🛠 Actions Taken
- Reset CMOS using both jumper and clear switch
- Reseated GPU and RAM
- Verified all power cables were fully inserted

---

## 🧾 Notes and Lessons

- OEM boards often have **non-standard front panel connectors** (13-pin, no labels)
- Always connect **monitor to GPU** once a discrete card is installed
- **Clear CMOS** after GPU/PSU swap if no video signal
- Some RTX 1650 cards won't work with legacy BIOS — UEFI may be required
- Lenovo boards may resist booting with newer GPUs without special BIOS updates

---

## 📌 Status

- **System powers on**
- **GPU installed and powered**
- **No display output (as of last test)**

---

## ✅ Next Steps (Optional)

- Try RTX 1650 in another system to rule out GPU issue
- Test with a known-good GPU in the Lenovo (e.g., GT 710 or RX 550)
- Consider upgrading to a newer board+CPU combo using same PSU + GPU
