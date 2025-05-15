<h1 align="center">👋 Hi, I'm Abel Amare</h1>
<h3 align="center">Software Engineering Student at Bahir Dar University | Passionate about Web Development, Linux, and System Programming</h3>

<p align="center">
  <a href="https://github.com/codebyabel/OSSP-KWORTLINUX-Abel/stargazers" target="_blank">
    <img src="https://img.shields.io/github/stars/codebyabel/OSSP-KWORTLINUX-Abel?style=social" alt="Stars">
  </a>
  <a href="https://github.com/codebyabel/OSSP-KWORTLINUX-Abel/network/members" target="_blank">
    <img src="https://img.shields.io/github/forks/codebyabel/OSSP-KWORTLINUX-Abel?style=social" alt="Forks">
  </a>
  <img src="https://visitor-badge.laobi.icu/badge?page_id=codebyabel.codebyabel" alt="Visitors">
</p>

---

## 📌 Project: OSSP – Installing Kwort Linux & Implementing exec() System Call

> This project is part of the Operating Systems and System Programming (OSSP) course at Bahir Dar University. It involves installing Kwort Linux on VMware, configuring its environment, and implementing the `exec()` system call in C.

---

## 🧭 Table of Contents

- 🔰 Introduction  
- 🎯 Objectives  
- 🖥️ System Requirements  
  - Hardware Requirements  
  - Software Requirements  
- 🛠️ Installation Steps  
  - VMware Setup  
  - Kwort Linux Installation  
  - GRUB Configuration  
  - Network Setup  
  - GUI Installation  
- ⚠️ Issues Faced  
- ✔️ Solutions Applied  
- 📁 Filesystem Support  
- ✅ Advantages & ❌ Disadvantages  
- 📌 Conclusion  
- 🔮 Future Outlook / Recommendations  

---

## 🔰 Introduction

The OSSP project explores how to manually install a lightweight Linux distribution (Kwort) in a virtualized environment, providing insights into Linux bootloaders, services, and system-level programming using system calls like `exec()`.

---

## 🎯 Objectives

- Understand the installation of Linux using VMware.
- Learn how to configure Linux networking, GUI, and services.
- Implement a system call (`exec()`) using C.
- Analyze filesystem and OS behavior.
- Compare virtualization technologies.

---

## 🖥️ System Requirements

### Hardware Requirements
- 4 GB RAM minimum
- 25 GB free disk space
- Dual-core processor or higher
- Virtualization-enabled BIOS

### Software Requirements
- VMware Workstation / VMware Player
- Kwort Linux ISO
- GCC compiler
- Optional: `lxdm`, `xfce4`, `dhcpcd`

---

## 🛠️ Installation Steps

### VMware Setup
- Created a new VM with recommended specs.
- Mounted Kwort ISO as a boot medium.

### Kwort Linux Installation
- Manually partitioned disk using `cfdisk`.
- Formatted using `mkfs.ext4` and mounted partitions.
- Installed base system via `kwort-install`.

### GRUB Configuration
- Installed GRUB with `grub-install /dev/sda`.
- Generated GRUB config using `grub-mkconfig -o /boot/grub/grub.cfg`.

### Network Setup
- Configured `/etc/resolv.conf` manually for DNS.
- Verified connectivity using `ping`.

### GUI Installation (Optional)
```bash
kpkg update
kpkg install xfce4 lxdm
