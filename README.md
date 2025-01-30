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


# **Linux Special Characters and Variables Guide**

This document provides a comprehensive overview of **special characters** in Linux, along with **variable types**, their definitions, and modifications.

---

## **1. Special Characters in Linux**

| Character | Description | Example |
|-----------|-------------|---------|
| `#` | Comment in shell scripts | `# This is a comment` |
| `$` | Variable expansion | `echo $HOME` |
| `*` | Wildcard for matching multiple files | `ls *.txt` |
| `?` | Wildcard for single character match | `ls file?.txt` |
| `~` | Home directory shortcut | `cd ~/Documents` |
| `&` | Run process in background | `sleep 10 &` |
| `;` | Command separator | `cd /tmp; ls` |
| `|` | Pipe command output | `ls | grep txt` |
| `>` | Redirect output to a file | `echo "Hello" > file.txt` |
| `>>` | Append output to a file | `echo "Hello" >> file.txt` |
| `<` | Redirect input from a file | `sort < file.txt` |
| `<<` | Here document for multi-line input | `cat << EOF` |
| `>` | Redirect standard output | `ls > output.txt` |
| `2>` | Redirect error output | `ls nonfile 2> error.log` |
| `&&` | Execute next command if previous succeeds | `mkdir test && cd test` |
| `||` | Execute next command if previous fails | `mkdir test || echo "Failed"` |
| `()` | Execute command in a subshell | `(cd /tmp && ls)` |
| `{}` | Group commands | `{ echo "First"; echo "Second"; }` |
| `$(command)` | Command substitution | `echo $(date)` |
| `` `command` `` | Alternative command substitution | `` echo `date` `` |
| `\` | Escape special characters | `echo "\$HOME"` |
| `:` | No operation (used in scripts) | `: do nothing` |
| `!` | Negate a command or history expansion | `!ls` |

---

## **2. Variable Types in Linux**

### **2.1 Local Variables**
- Defined within a script/session and not inherited by child processes.
- Example:
  ```bash
  myvar="Hello"
  echo $myvar
  ```

### **2.2 Environment Variables**
- Available system-wide and inherited by child processes.
- Example:
  ```bash
  export MY_ENV="Global Variable"
  ```
  
### **2.3 Shell Variables**
- Special variables set by the shell, affecting its behavior.
- Example:
  ```bash
  echo $SHELL   # Shows current shell
  echo $PATH    # Shows executable search paths
  ```

---

## **3. Defining and Modifying Variables**

| Operation | Command | Example |
|-----------|----------|---------|
| Define a variable | `VAR=value` | `myvar="Hello"` |
| Access variable | `$VAR` | `echo $myvar` |
| Export variable | `export VAR=value` | `export PATH=$PATH:/opt/bin` |
| Remove variable | `unset VAR` | `unset myvar` |
| Append to variable | `VAR+="value"` | `PATH+=":/opt/bin"` |
| Read user input | `read VAR` | `read username` |
| Assign output of command | `VAR=$(command)` | `NOW=$(date)` |
| Check if variable is set | `${VAR:-default}` | `echo ${HOME:-"/home/default"}` |
| Check if variable is empty | `${VAR:+value}` | `echo ${HOME:+"Set"}` |

---

## **4. Special Shell Variables**

| Variable | Description |
|----------|-------------|
| `$0` | Name of the script |
| `$1, $2, ...` | Positional parameters |
| `$@` | All parameters as separate words |
| `$*` | All parameters as a single string |
| `$#` | Number of arguments passed to script |
| `$?` | Exit status of last command |
| `$$` | Process ID of the current script |
| `$!` | Process ID of last background command |
| `$_` | Last argument of last command |

---

This guide serves as a reference for **special characters**, **variables**, and **shell scripting essentials** in Linux. 🚀



