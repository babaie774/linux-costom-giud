# 📁 Linux Directory Structure - The Ultimate Guide

Linux follows the **Filesystem Hierarchy Standard (FHS)**, which defines how files and directories are structured. This guide explains **every possible directory** in detail, including rare and advanced directories.

---

## 📌 Root Directory (`/`)

Everything in Linux starts from the root directory (`/`). All other directories and files branch out from here.

| Directory | Description |
|-----------|-------------|
| `/bin` | Essential user binaries (e.g., `ls`, `cp`, `mv`, `rm`, `echo`). |
| `/sbin` | System binaries (e.g., `fsck`, `shutdown`, `reboot`). |
| `/boot` | Contains the boot loader (`GRUB`), Linux kernel, and initial RAM disk (`initrd`). |
| `/dev` | Device files representing hardware (`/dev/sda` for disks, `/dev/null`). |
| `/etc` | System-wide configuration files (`passwd`, `fstab`, `hosts`). |
| `/home` | Home directories for users (`/home/user`). |
| `/lib` | Essential shared libraries needed by binaries in `/bin` and `/sbin`. |
| `/lib64` | Shared 64-bit libraries (on 64-bit systems). |
| `/media` | Mount point for removable storage (USB, CDs, DVDs). |
| `/mnt` | Temporary mount point for manually mounted filesystems. |
| `/opt` | Optional software and third-party applications. |
| `/proc` | Virtual filesystem providing system information (CPU, memory, processes). |
| `/root` | Home directory for the root user. |
| `/run` | Runtime process data and process ID (PID) files. |
| `/srv` | Data for services (e.g., web servers, FTP, databases). |
| `/sys` | Virtual filesystem containing system and hardware information. |
| `/tmp` | Temporary files (deleted on reboot). |
| `/usr` | Secondary hierarchy containing user programs, libraries, and documentation. |
| `/var` | Variable data such as logs, caches, mail, and databases. |

---

## 📂 Detailed Breakdown of All Directories and Subdirectories

### 🔹 `/bin` - Essential User Binaries
Contains core utilities needed for the system to function.

| File | Description |
|------|------------|
| `/bin/ls` | List files in a directory. |
| `/bin/cp` | Copy files and directories. |
| `/bin/mv` | Move or rename files. |
| `/bin/rm` | Remove files and directories. |
| `/bin/cat` | Display file contents. |

---

### 🔹 `/sbin` - System Binaries
System utilities for system administration.

| File | Description |
|------|------------|
| `/sbin/fsck` | Filesystem check and repair tool. |
| `/sbin/mount` | Mount filesystems. |
| `/sbin/reboot` | Reboot the system. |

---

### 🔹 `/boot` - Boot Loader and Kernel Files
Contains everything needed for the system to boot.

| File | Description |
|------|------------|
| `/boot/vmlinuz` | Compressed Linux kernel. |
| `/boot/initrd.img` | Initial RAM disk used at boot. |
| `/boot/grub/grub.cfg` | GRUB bootloader configuration. |

---

### 🔹 `/dev` - Device Files
Contains special files representing devices.

| File | Description |
|------|------------|
| `/dev/sda` | First hard disk. |
| `/dev/null` | A "black hole" where data is discarded. |
| `/dev/random` | Random number generator. |
| `/dev/tty` | Terminal devices. |

---

### 🔹 `/etc` - Configuration Files
Contains global configuration files for the system and services.

| File | Description |
|------|------------|
| `/etc/passwd` | User account details. |
| `/etc/shadow` | Encrypted passwords. |
| `/etc/fstab` | Filesystem mount information. |
| `/etc/hosts` | Static hostname-to-IP mapping. |
| `/etc/crontab` | Scheduled tasks (cron jobs). |

---

### 🔹 `/home` - User Home Directories
Each user gets a home directory (`/home/username`) to store personal files.

| Directory | Description |
|-----------|------------|
| `/home/user/` | Personal files, documents, and configurations. |
| `/home/user/.bashrc` | User’s Bash shell configuration. |

---

### 🔹 `/lib` and `/lib64` - Shared Libraries
Contains essential shared libraries needed for system binaries.

| Directory | Description |
|-----------|------------|
| `/lib/modules/` | Kernel modules. |
| `/lib/firmware/` | Device firmware. |

---

### 🔹 `/media` and `/mnt` - Mount Points
Used for mounting external drives.

| Directory | Description |
|-----------|------------|
| `/media/usb` | Mounted USB drive. |
| `/media/cdrom` | Mounted CD-ROM. |
| `/mnt/temp` | Manually mounted filesystem. |

---

### 🔹 `/opt` - Optional Software
Stores manually installed software and third-party applications.

| Directory | Description |
|-----------|------------|
| `/opt/google/` | Google Chrome installation files. |
| `/opt/vscode/` | VS Code installation files. |

---

### 🔹 `/proc` - Virtual Filesystem for System Information
Provides dynamic system information.

| File | Description |
|------|------------|
| `/proc/cpuinfo` | CPU details. |
| `/proc/meminfo` | Memory usage details. |
| `/proc/uptime` | System uptime. |

---

### 🔹 `/root` - Root User’s Home Directory
The home directory for the superuser (`root`).

---

### 🔹 `/run` - Runtime Data
Contains temporary system runtime data.

| File | Description |
|------|------------|
| `/run/utmp` | Information about logged-in users. |
| `/run/systemd/` | Systemd process data. |

---

### 🔹 `/srv` - Service Data
Used for server-related files.

| Directory | Description |
|-----------|------------|
| `/srv/http/` | Web server files. |
| `/srv/ftp/` | FTP server files. |

---

### 🔹 `/sys` - System and Hardware Information
Contains system and hardware information.

| Directory | Description |
|-----------|------------|
| `/sys/class/` | Hardware classification. |
| `/sys/block/` | Storage device information. |

---

### 🔹 `/tmp` - Temporary Files
Stores temporary files created by applications.

| File | Description |
|------|------------|
| `/tmp/somefile.tmp` | A temporary file. |

---

### 🔹 `/usr` - User Programs and Libraries
Contains installed software, documentation, and utilities.

| Directory | Description |
|-----------|------------|
| `/usr/bin/` | User executables (`nano`, `vim`, `wget`). |
| `/usr/lib/` | Shared libraries. |
| `/usr/share/` | Architecture-independent data. |

---

### 🔹 `/var` - Variable Data Files
Stores variable data like logs, mail, and databases.

| Directory | Description |
|-----------|------------|
| `/var/log/` | System logs (`syslog`, `auth.log`). |
| `/var/mail/` | User emails. |
| `/var/cache/` | Cached application data. |
| `/var/www/` | Web server files (Apache, Nginx). |

---

## ✅ Final Summary - Mastering Linux Directories

- **System essentials** → `/bin`, `/sbin`, `/lib`, `/boot`
- **User-related files** → `/home`, `/root`
- **Configuration & services** → `/etc`, `/opt`, `/srv`
- **Devices & system info** → `/dev`, `/sys`, `/proc`
- **Mount points & storage** → `/mnt`, `/media`
- **Temporary & runtime** → `/tmp`, `/run`
- **Installed software & apps** → `/usr`, `/var`

---

This guide **covers every possible directory** in Linux, giving you complete mastery over the Linux filesystem! 🚀🔥



# **Linux Command Guide**

This document provides a comprehensive list of essential Linux commands categorized based on functionality.

---

## **1. Kernel Commands**

| Command | Description | Example |
|---------|-------------|---------|
| `uname -r` | Display the kernel version | `uname -r` |
| `uname -a` | Show all system information | `uname -a` |
| `dmesg` | Display kernel messages | `dmesg | less` |
| `sysctl -a` | Show all kernel parameters | `sysctl -a` |
| `sysctl -w` | Modify kernel parameters at runtime | `sysctl -w net.ipv4.ip_forward=1` |
| `modprobe` | Load a kernel module | `modprobe module_name` |
| `rmmod` | Remove a kernel module | `rmmod module_name` |
| `lsmod` | List currently loaded kernel modules | `lsmod` |
| `cat /proc/version` | Show kernel version and build details | `cat /proc/version` |

---

## **2. Hardware Commands**

| Command | Description | Example |
|---------|-------------|---------|
| `lshw` | Display detailed hardware info | `sudo lshw -short` |
| `lscpu` | Show CPU details | `lscpu` |
| `lsblk` | List information about block devices | `lsblk` |
| `df -h` | Show disk space usage | `df -h` |
| `free -h` | Display memory usage | `free -h` |
| `lsusb` | List USB devices | `lsusb` |
| `lspci` | List PCI devices | `lspci` |
| `dmidecode` | Show system hardware information | `sudo dmidecode` |
| `hdparm -I /dev/sda` | Display hard drive information | `sudo hdparm -I /dev/sda` |
| `uptime` | Show system uptime | `uptime` |

---

## **3. Operating System Commands**

| Command | Description | Example |
|---------|-------------|---------|
| `hostnamectl` | Display system hostname info | `hostnamectl` |
| `uptime` | Show system uptime | `uptime` |
| `lsb_release -a` | Get Linux distribution details | `lsb_release -a` |
| `cat /etc/os-release` | Display OS version | `cat /etc/os-release` |
| `whoami` | Show current user | `whoami` |
| `env` | Display environment variables | `env` |
| `date` | Show system date and time | `date` |
| `cal` | Display a calendar | `cal` |

---

## **4. Networking Commands**

| Command | Description | Example |
|---------|-------------|---------|
| `ip a` | Show IP addresses | `ip a` |
| `ifconfig` | Display network interfaces (deprecated) | `ifconfig` |
| `ip route` | Show routing table | `ip route` |
| `ping` | Test network connectivity | `ping google.com` |
| `netstat -tulnp` | List open ports and services | `netstat -tulnp` |
| `ss -tulnp` | Show listening sockets | `ss -tulnp` |
| `nslookup` | Query DNS records | `nslookup google.com` |
| `dig` | Perform DNS lookups | `dig google.com` |
| `traceroute` | Trace route to a host | `traceroute google.com` |

---

## **5. Process and Service Management**

| Command | Description | Example |
|---------|-------------|---------|
| `ps aux` | Show running processes | `ps aux` |
| `top` | Display real-time processes | `top` |
| `htop` | Enhanced process viewer | `htop` |
| `systemctl status` | Show service status | `systemctl status apache2` |
| `systemctl start` | Start a service | `systemctl start apache2` |
| `systemctl stop` | Stop a service | `systemctl stop apache2` |
| `systemctl restart` | Restart a service | `systemctl restart apache2` |
| `systemctl enable` | Enable service at boot | `systemctl enable apache2` |
| `systemctl disable` | Disable service at boot | `systemctl disable apache2` |
| `kill -9 PID` | Terminate a process | `kill -9 1234` |
| `nice -n 10 command` | Run command with priority | `nice -n 10 make` |

---

This guide serves as a reference for essential Linux commands, categorized for ease of use. 🚀


