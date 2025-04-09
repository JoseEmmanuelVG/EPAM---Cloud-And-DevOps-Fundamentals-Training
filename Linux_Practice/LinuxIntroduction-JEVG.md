# 📘 Linux Introduction Notes: Key Concepts and Topics

## 🟡 1. Unix-Based OS and Linux Distributions
### Origin of Linux:
- **Linux** is a free and open-source operating system inspired by **MINIX**, a Unix-like OS designed for educational purposes by Andrew S. Tanenbaum.
- Created by **Linus Torvalds** in 1991.
- Built as a **Unix-like** system but developed from scratch without using MINIX code.
- Promoted under the **GNU General Public License (GPL)**.

### Linux Distributions:
- **Linux Distribution (Distro)**: A complete operating system package built around the Linux kernel.
- Popular Distros:
  - **Ubuntu:** User-friendly, great for beginners.
  - **Debian:** Stable and reliable, used as a base for many distros.
  - **CentOS/RHEL:** Enterprise-focused, stable for servers.
  - **Arch Linux:** Rolling release, suitable for advanced users.
  - **Fedora:** Cutting-edge technology, often used for development.

---

## 🟡 2. Linux Startup Process and Boot Loaders
The Linux startup sequence involves several stages:

### **Startup Process Stages:**
1. **BIOS/UEFI:** Initializes hardware and passes control to the bootloader.
2. **Bootloader:** Loads the kernel into memory. Examples include:
   - **GRUB (GRand Unified Bootloader):** Most common in modern Linux distributions.
   - **LILO (Linux Loader):** An older bootloader.
3. **Kernel:** The core of the operating system. Manages hardware, processes, and memory.
4. **Init System (e.g., `systemd`):** Manages services and runlevels.
5. **Shell:** Provides a command-line interface for user interaction.

### 📌 **Common Boot Loaders:**
- **GRUB (GRand Unified Bootloader):** Default for most Linux distributions.
- **LILO (Linux Loader):** Older, replaced by GRUB in modern systems.

### 🚫 **Not Boot Loaders:**
- **LIFO (Last-In, First-Out):** A queue structure, not a boot loader.
- **FIFO (First-In, First-Out):** Another queue structure, unrelated to boot loading.

---

## 🟡 3. Shell – User Interaction with the OS
### **What is a Shell?**
The **Shell** is a program that acts as an intermediary between the user and the kernel. It interprets commands and executes them.

### **Types of Shells:**
- **Bash (Bourne Again Shell):** Default in many Linux distributions.
- **Zsh:** Advanced features like plugins and themes.
- **Fish:** User-friendly and interactive.
- **Sh:** Original Bourne shell.

### **Common Shell Commands:**
- `ls` – List files and directories.
- `cd` – Change directory.
- `mkdir` – Create a directory.
- `cp` – Copy files.
- `rm` – Remove files or directories.
- `echo` – Display text or variables.

---

## 🟡 4. File Systems
### **Linux and File Extensions:**
- **Linux does not rely on file extensions** to determine file types. Instead, it inspects the file's contents or metadata.

### **How to Identify File Types:**
- `file <filename>` – Displays the type of a file.
- `ls -l` – Displays file details.
- `stat <filename>` – Shows detailed file status.

### **Common File Systems Used in Linux:**
- **EXT2 (Second Extended Filesystem):** Early standard, lacks journaling.
- **EXT3 (Third Extended Filesystem):** Adds journaling for better crash recovery.
- **EXT4 (Fourth Extended Filesystem):** Modern standard, supports large files and volumes.
- **ReiserFS:** Known for fast handling of small files.
- **XFS:** High-performance file system, often used for large storage servers.

### **File Systems Not Native to Linux:**
- **NTFS:** Default file system for Windows.
- **FAT32:** Older, cross-platform file system.

---

## 🟡 5. Disk Quotas
**Disk Quotas** are limits set by administrators to control the amount of disk space and the number of files that users or groups can use.

### **Key Commands for Disk Quotas:**
- Enable quota on a filesystem:
  ```bash
  sudo mount -o remount,usrquota,grpquota /home

- Initialize quota database:
  ```bash
  sudo quotacheck -cum /home

- Assign quota to a user:
  ```bash
  sudo edquota -u username

- View user quota:
  ```bash
  quota -u username


  
---
<details>
  <summary>🌟 Did you find any repository useful?</summary>
  If any project has been helpful to you, consider giving it a ⭐ star in the repository and follow my GitHub account to stay tuned for future updates! 🚀

  In addition, I am always open to suggestions, recommendations or collaborations. Feel free to [get in touch](https://www.linkedin.com/in/vazquez-galan-jose-emmanuel-664968221) if you have any questions or ideas for improving this project. I'm excited for your feedback and contributions.

  Thank you for your interest and support! 😊
</details>




<p align="center">
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.
</p>

