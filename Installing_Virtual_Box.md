# 💻 Installing VirtualBox & Ubuntu on Microsoft Surface Pro

This document outlines the steps I followed to install VirtualBox on my Microsoft Surface Pro and set up Ubuntu 24.04.2 in a virtual machine.

---

## 🧭 Process Overview

1. **Downloaded VirtualBox**  
   - Searched using [Bing for VirtualBox](https://www.bing.com/search?pglt=2337&q=virtualbox&cvid=c26ea576708f4a78ab82d9f8844bb551&gs_lcrp=EgRlZGdlKgkIABBFGDsY-QcyCQgAEEUYOxj5BzIGCAEQRRg5MgYIAhBFGDwyBggDEEUYPDIGCAQQRRg9MgYIBRBFGDwyBggGEEUYPNIBCDEwNTBqMGoxqAIAsAIA&FORM=ANNTA1&PC=U531)

2. **C++ Redistributable Missing Error**  
   - Encountered an error due to missing C++ 2019 runtime.
   - Downloaded it from the official Microsoft page:  
     [Visual C++ Redistributables – Microsoft Docs](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170)

3. **Successfully Installed VirtualBox**

4. **Chose Ubuntu as the OS**  
   - Downloaded Ubuntu 24.04.2 (x64) from:  
     [Ubuntu Desktop Download](https://ubuntu.com/download/desktop#newsletter-signup)

---

## 🧰 Installing Ubuntu in VirtualBox

1. **Create New Virtual Machine**
   - Name: Ubuntu
   - Type: Linux
   - Version: Ubuntu (64-bit)

2. **Configure VM Settings**
   - Set CPU and memory allocation
   - Set storage size

3. **Attach ISO File**
   - Go to `Settings → Storage`
   - Select the empty optical drive
   - Click the disk icon and choose the Ubuntu `.iso` file

---

## 🖼️ Screenshots

![VirtualBox Setup Screenshot 1](https://github.com/user-attachments/assets/c8c4c136-a839-45ea-ac2e-ec7342ee5454)

![VirtualBox Setup Screenshot 2](https://github.com/user-attachments/assets/053a6b6e-df83-4873-8d43-a7a9ea88f918)

---

## 📝 Notes to Self

- Always install Visual C++ dependencies if VirtualBox fails during install
- Allocate at least 2 CPUs and 4GB RAM for smoother Ubuntu performance
- Consider enabling 3D acceleration under `Display` settings
- Snapshot the VM once Ubuntu is installed and configured
