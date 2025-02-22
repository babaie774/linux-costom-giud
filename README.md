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

# **Comprehensive Guide to File and Directory Commands in Linux**

This document provides a detailed list of commands for working with files and directories in Linux, along with their options.

---

## **1. Listing Files and Directories**
| Command | Description | Example |
|---------|-------------|---------|
| `ls` | List files in a directory | `ls` |
| `ls -l` | Long format listing with details | `ls -l` |
| `ls -a` | Show hidden files | `ls -a` |
| `ls -lh` | Show file sizes in human-readable format | `ls -lh` |
| `ls -R` | List directories recursively | `ls -R` |
| `ls -t` | Sort files by modification time | `ls -lt` |

---

## **2. Creating Files and Directories**
| Command | Description | Example |
|---------|-------------|---------|
| `touch filename` | Create an empty file | `touch file.txt` |
| `mkdir dirname` | Create a new directory | `mkdir new_folder` |
| `mkdir -p dir1/dir2` | Create nested directories | `mkdir -p projects/work` |

---

## **3. Removing Files and Directories**
| Command | Description | Example |
|---------|-------------|---------|
| `rm filename` | Remove a file | `rm file.txt` |
| `rm -r dirname` | Remove a directory and its contents | `rm -r folder` |
| `rm -f filename` | Force remove a file without confirmation | `rm -f file.txt` |
| `rmdir dirname` | Remove an empty directory | `rmdir empty_folder` |

---

## **4. Copying Files and Directories**
| Command | Description | Example |
|---------|-------------|---------|
| `cp file1 file2` | Copy a file | `cp file.txt backup.txt` |
| `cp -r dir1 dir2` | Copy a directory recursively | `cp -r folder1 folder2` |
| `cp -i file1 file2` | Prompt before overwriting | `cp -i file.txt backup.txt` |
| `cp -u file1 file2` | Copy only if source is newer | `cp -u file1 file2` |

---

## **5. Moving and Renaming Files**
| Command | Description | Example |
|---------|-------------|---------|
| `mv file1 file2` | Rename a file | `mv old.txt new.txt` |
| `mv file1 dir/` | Move a file to a directory | `mv file.txt backup/` |
| `mv -i file1 file2` | Prompt before overwriting | `mv -i file1 file2` |

---

## **6. Finding Files and Directories**
| Command | Description | Example |
|---------|-------------|---------|
| `find /path -name filename` | Find files by name | `find /home -name "file.txt"` |
| `find /path -type d` | Find directories only | `find /home -type d` |
| `find /path -size +100M` | Find files larger than 100MB | `find /var/log -size +100M` |
| `locate filename` | Locate a file quickly (requires `updatedb`) | `locate file.txt` |
| `updatedb` | Update the locate database | `sudo updatedb` |

---

## **7. Viewing File Contents**
| Command | Description | Example |
|---------|-------------|---------|
| `cat filename` | Display file contents | `cat file.txt` |
| `tac filename` | Display file in reverse | `tac file.txt` |
| `less filename` | View file content one page at a time | `less file.txt` |
| `head -n 10 filename` | Show first 10 lines | `head -n 10 file.txt` |
| `tail -n 10 filename` | Show last 10 lines | `tail -n 10 file.txt` |
| `tail -f filename` | Continuously watch a file | `tail -f log.txt` |

---

## **8. Editing and Manipulating Files**
| Command | Description | Example |
|---------|-------------|---------|
| `echo "text" > file` | Write text to a file (overwrite) | `echo "Hello" > file.txt` |
| `echo "text" >> file` | Append text to a file | `echo "World" >> file.txt` |
| `sed -i 's/old/new/g' filename` | Replace text in a file | `sed -i 's/foo/bar/g' file.txt` |
| `awk '{print $1}' filename` | Extract the first column from a file | `awk '{print $1}' data.txt` |
| `cut -d':' -f1 filename` | Extract first field using `:` delimiter | `cut -d':' -f1 /etc/passwd` |

---

## **9. Changing Permissions and Ownership**
| Command | Description | Example |
|---------|-------------|---------|
| `chmod 644 file` | Set read/write for owner, read for others | `chmod 644 file.txt` |
| `chmod 755 file` | Set executable for owner and read for others | `chmod 755 script.sh` |
| `chown user:group file` | Change owner and group of a file | `chown user1:group1 file.txt` |
| `chgrp group file` | Change group ownership | `chgrp users file.txt` |

---

## **10. Creating and Extracting Archives**
| Command | Description | Example |
|---------|-------------|---------|
| `tar -cvf archive.tar files` | Create a tar archive | `tar -cvf backup.tar folder/` |
| `tar -xvf archive.tar` | Extract a tar archive | `tar -xvf backup.tar` |
| `tar -czvf archive.tar.gz files` | Create a compressed tar.gz archive | `tar -czvf backup.tar.gz folder/` |
| `tar -xzvf archive.tar.gz` | Extract a tar.gz archive | `tar -xzvf backup.tar.gz` |
| `zip -r archive.zip folder/` | Create a zip archive | `zip -r backup.zip folder/` |
| `unzip archive.zip` | Extract a zip archive | `unzip backup.zip` |

---

## **11. Disk Usage and Space Management**
| Command | Description | Example |
|---------|-------------|---------|
| `df -h` | Show free disk space | `df -h` |
| `du -sh dir` | Show directory size | `du -sh /home` |
| `du -ah` | Show size of all files | `du -ah /var/log` |
| `find / -size +1G` | Find files larger than 1GB | `find / -size +1G` |

---

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
  env   # Display all environment variables
  printenv   # Print all environment variables
  set   # Show all shell variables (including environment variables)
  export   # Show exported environment variables

  export VAR_NAME=value   # Set an environment variable for the current session
  echo $VAR_NAME   # Check if a variable exists
  unset VAR_NAME   # Remove an environment variable
  
  echo $PATH   # Show current PATH
  export PATH=$PATH:/new/directory   # Append a directory to PATH


  echo 'export VAR_NAME=value' >> ~/.bashrc   # Add to ~/.bashrc for persistence source ~/.bashrc   # Apply changes
  ```
  
### **2.3 Shell Variables**
- Special variables set by the shell, affecting its behavior.
- Example:
  ```bash
  echo $SHELL   # Shows current shell
  echo $PATH    # Shows executable search paths
  echo $SHELL   # Shows current shell
  getent passwd $USER | cut -d: -f7   # Alternative way to get the shell
  chsh -l   # List available shells
  
  echo $HOME   # Shows the user's home directory
  eval echo ~$USER   # Alternative way to get the home directory
  getent passwd $USER | cut -d: -f6   # Another way to retrieve home directory
  
  echo $USER   # Shows the current logged-in user
  whoami   # Alternative way to get the user
  id -un   # Another way to retrieve the username
  
  echo $PWD   # Shows the current working directory
  pwd   # Alternative way to get the current directory
  
  echo $PATH   # Shows executable search paths
  printenv PATH   # Alternative way to get the PATH
  env | grep PATH   # Another way to display the PATH
  
  echo $EDITOR   # Shows the default text editor
  update-alternatives --display editor   # List available editors
  
  echo $LANG   # Shows the system language
  locale   # Display locale settings
  
  echo $HOSTNAME   # Shows the system hostname
  hostname   # Alternative way to get the hostname
  uname -n   # Another way to retrieve the hostname
  
  echo $UID   # Shows the user ID
  id -u   # Alternative way to get the user ID
  
  echo $GID   # Shows the group ID
  id -g   # Alternative way to get the group ID
  
  echo $LOGNAME   # Shows the logged-in username
  logname   # Alternative way to get the username
  
  echo $TERM   # Shows the current terminal type
  tput longname   # Alternative way to describe the terminal
  
  echo $DISPLAY   # Shows the X display server used (for GUI sessions)
  xdpyinfo | grep display   # Alternative way to check display
  
  echo $XDG_SESSION_TYPE   # Shows if session is GUI or terminal
  loginctl show-session $(loginctl | grep $USER | awk '{print $1}') -p Type   # Alternative way to check session type
  
  echo $XDG_CURRENT_DESKTOP   # Shows the current desktop environment
  echo $DESKTOP_SESSION   # Alternative way to check desktop session
  
  echo $SHLVL   # Shows the shell nesting level
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

## **5. Special Characters in Linux**

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

## **1. File Globbing in Linux**
File globbing is used for **pattern matching in filenames and paths** within shell commands. It utilizes special wildcard characters to match files.

### **Common Glob Patterns**
| Pattern | Description | Example |
|---------|-------------|---------|
| `*` | Matches any number of characters (including none) | `ls *.txt` (lists all `.txt` files) |
| `?` | Matches a single character | `ls file?.txt` (matches `file1.txt`, `file2.txt`, etc.) |
| `[abc]` | Matches **any one** of the specified characters | `ls file[123].txt` (matches `file1.txt`, `file2.txt`, `file3.txt`) |
| `[a-z]` | Matches any single character in the specified range | `ls file[a-d].txt` (matches `filea.txt` to `filed.txt`) |
| `[!abc]` | Matches any character **except** the specified ones | `ls file[!123].txt` (excludes `file1.txt`, `file2.txt`, `file3.txt`) |
| `{a,b,c}` | Matches any **comma-separated values** within `{}` | `ls file{1,2,3}.txt` (matches `file1.txt`, `file2.txt`, `file3.txt`) |
| `**` | Matches directories recursively (Bash 4.0+) | `ls **/*.txt` (finds `.txt` files in all subdirectories) |

### **Globbing Examples**
```sh
ls *.sh          # List all shell scripts
rm file?.txt     # Remove files like file1.txt, file2.txt
mv doc[1-3].pdf backup/  # Move doc1.pdf, doc2.pdf, doc3.pdf to backup/
```

---

## **2. Regular Expressions (Regex) in Linux**
Regular expressions provide powerful **pattern matching capabilities** beyond file globbing and are commonly used in tools like `grep`, `sed`, `awk`, and `find`.

### **Basic Regular Expression Syntax**
| Pattern | Description | Example |
|---------|-------------|---------|
| `.` | Matches **any single character** except a newline | `grep "b.g" file.txt` (matches `bag`, `bog`, `big`) |
| `^` | Matches the **beginning** of a line | `grep "^Hello" file.txt` (matches lines starting with `Hello`) |
| `$` | Matches the **end** of a line | `grep "world$" file.txt` (matches lines ending with `world`) |
| `*` | Matches **zero or more** occurrences of the preceding character | `grep "ab*" file.txt` (matches `a`, `ab`, `abb`, `abbb`, etc.) |
| `+` | Matches **one or more** occurrences of the preceding character | `grep "ab+" file.txt` (matches `ab`, `abb`, `abbb`, but not `a`) |
| `?` | Matches **zero or one** occurrences of the preceding character | `grep "colou?r" file.txt` (matches `color` and `colour`) |
| `{n}` | Matches **exactly n** occurrences of the preceding character | `grep "a{3}" file.txt` (matches `aaa`) |
| `{n,}` | Matches **at least n** occurrences | `grep "a{2,}" file.txt` (matches `aa`, `aaa`, `aaaa`, etc.) |
| `{n,m}` | Matches **between n and m** occurrences | `grep "a{2,4}" file.txt` (matches `aa`, `aaa`, `aaaa`) |
| `[abc]` | Matches **any one** of the specified characters | `grep "[aeiou]" file.txt` (matches vowels) |
| `[^abc]` | Matches **any character except** the ones inside `[]` | `grep "[^0-9]" file.txt` (matches non-digit characters) |
| `(abc)` | Groups a subpattern | `grep "(hello|world)" file.txt` (matches `hello` or `world`) |
| `\` | Escape special characters | `grep "\.txt" file.txt` (matches `.txt`) |

### **Extended Regular Expressions (ERE) with `grep -E`**
```sh
grep -E "colou?r" file.txt   # Matches 'color' or 'colour'
grep -E "[0-9]{2,4}" file.txt  # Matches numbers with 2 to 4 digits
grep -E "^Start.*end$" file.txt  # Matches lines starting with 'Start' and ending with 'end'
```

### **Regex with `sed` for Text Manipulation**
```sh
sed -E 's/[0-9]+/NUMBER/g' file.txt   # Replace all numbers with 'NUMBER'
sed -E 's/(hello|hi)/HEY/g' file.txt  # Replace 'hello' or 'hi' with 'HEY'
```

### **Regex with `awk` for Text Processing**
```sh
awk '/error/ {print $0}' log.txt    # Print lines containing 'error'
awk '/^[0-9]+/ {print $1}' data.txt  # Print first column if it starts with a number
```

---

## **3. Differences Between Globbing and Regex**
| Feature | Globbing | Regular Expressions |
|---------|---------|------------------|
| Used for | Matching file names | Matching patterns in text |
| Wildcards | `*`, `?`, `[]`, `{}` | `^`, `$`, `.` , `+`, `?`, `{}` |
| Tools | Shell (`ls`, `rm`, `cp`) | `grep`, `sed`, `awk`, `find` |
| Complexity | Simple | Advanced & powerful |

---

## **4. Practical Use Cases**
### **Find and Delete Files with Globbing**
```sh
rm *.log            # Delete all log files
find /var/log -name "*.log" -delete  # Find and delete all log files recursively
```

### **Find Files Using Regex in `grep`**
```sh
grep -E "error|fail" logs.txt  # Find lines containing 'error' or 'fail'
```

### **Replace Text Using `sed`**
```sh
sed -E 's/[0-9]+/NUM/' file.txt  # Replace numbers with 'NUM'
```

---

This guide provides essential knowledge of **file globbing** and **regular expressions** in Linux. 🚀


# **Linux File Globing and Regular Expressions Guide**

This document provides an overview of **file globbing** and **regular expressions (Regex)** in Linux, including syntax, examples, and common use cases.

---

## **1. File Globbing in Linux**
File globbing is used for **pattern matching in filenames and paths** within shell commands. It utilizes special wildcard characters to match files.

### **Common Glob Patterns**
| Pattern | Description | Example |
|---------|-------------|---------|
| `*` | Matches any number of characters (including none) | `ls *.txt` (lists all `.txt` files) |
| `?` | Matches a single character | `ls file?.txt` (matches `file1.txt`, `file2.txt`, etc.) |
| `[abc]` | Matches **any one** of the specified characters | `ls file[123].txt` (matches `file1.txt`, `file2.txt`, `file3.txt`) |
| `[a-z]` | Matches any single character in the specified range | `ls file[a-d].txt` (matches `filea.txt` to `filed.txt`) |
| `[!abc]` | Matches any character **except** the specified ones | `ls file[!123].txt` (excludes `file1.txt`, `file2.txt`, `file3.txt`) |
| `{a,b,c}` | Matches any **comma-separated values** within `{}` | `ls file{1,2,3}.txt` (matches `file1.txt`, `file2.txt`, `file3.txt`) |
| `**` | Matches directories recursively (Bash 4.0+) | `ls **/*.txt` (finds `.txt` files in all subdirectories) |

### **Globbing Examples**
```sh
ls *.sh          # List all shell scripts
rm file?.txt     # Remove files like file1.txt, file2.txt
mv doc[1-3].pdf backup/  # Move doc1.pdf, doc2.pdf, doc3.pdf to backup/
```

---

## **2. Regular Expressions (Regex) in Linux**
Regular expressions provide powerful **pattern matching capabilities** beyond file globbing and are commonly used in tools like `grep`, `sed`, `awk`, and `find`.

### **Basic Regular Expression Syntax**
| Pattern | Description | Example |
|---------|-------------|---------|
| `.` | Matches **any single character** except a newline | `grep "b.g" file.txt` (matches `bag`, `bog`, `big`) |
| `^` | Matches the **beginning** of a line | `grep "^Hello" file.txt` (matches lines starting with `Hello`) |
| `$` | Matches the **end** of a line | `grep "world$" file.txt` (matches lines ending with `world`) |
| `*` | Matches **zero or more** occurrences of the preceding character | `grep "ab*" file.txt` (matches `a`, `ab`, `abb`, `abbb`, etc.) |
| `+` | Matches **one or more** occurrences of the preceding character | `grep "ab+" file.txt` (matches `ab`, `abb`, `abbb`, but not `a`) |
| `?` | Matches **zero or one** occurrences of the preceding character | `grep "colou?r" file.txt` (matches `color` and `colour`) |
| `{n}` | Matches **exactly n** occurrences of the preceding character | `grep "a{3}" file.txt` (matches `aaa`) |
| `{n,}` | Matches **at least n** occurrences | `grep "a{2,}" file.txt` (matches `aa`, `aaa`, `aaaa`, etc.) |
| `{n,m}` | Matches **between n and m** occurrences | `grep "a{2,4}" file.txt` (matches `aa`, `aaa`, `aaaa`) |
| `[abc]` | Matches **any one** of the specified characters | `grep "[aeiou]" file.txt` (matches vowels) |
| `[^abc]` | Matches **any character except** the ones inside `[]` | `grep "[^0-9]" file.txt` (matches non-digit characters) |
| `(abc)` | Groups a subpattern | `grep "(hello|world)" file.txt` (matches `hello` or `world`) |
| `\` | Escape special characters | `grep "\.txt" file.txt` (matches `.txt`) |

### **Extended Regular Expressions (ERE) with `grep -E`**
```sh
grep -E "colou?r" file.txt   # Matches 'color' or 'colour'
grep -E "[0-9]{2,4}" file.txt  # Matches numbers with 2 to 4 digits
grep -E "^Start.*end$" file.txt  # Matches lines starting with 'Start' and ending with 'end'
```

### **Regex with `sed` for Text Manipulation**
```sh
sed -E 's/[0-9]+/NUMBER/g' file.txt   # Replace all numbers with 'NUMBER'
sed -E 's/(hello|hi)/HEY/g' file.txt  # Replace 'hello' or 'hi' with 'HEY'
```

### **Regex with `awk` for Text Processing**
```sh
awk '/error/ {print $0}' log.txt    # Print lines containing 'error'
awk '/^[0-9]+/ {print $1}' data.txt  # Print first column if it starts with a number
```

---

## **3. Differences Between Globbing and Regex**
| Feature | Globbing | Regular Expressions |
|---------|---------|------------------|
| Used for | Matching file names | Matching patterns in text |
| Wildcards | `*`, `?`, `[]`, `{}` | `^`, `$`, `.` , `+`, `?`, `{}` |
| Tools | Shell (`ls`, `rm`, `cp`) | `grep`, `sed`, `awk`, `find` |
| Complexity | Simple | Advanced & powerful |

---

## **4. Practical Use Cases**
### **Find and Delete Files with Globbing**
```sh
rm *.log            # Delete all log files
find /var/log -name "*.log" -delete  # Find and delete all log files recursively
```

### **Find Files Using Regex in `grep`**
```sh
grep -E "error|fail" logs.txt  # Find lines containing 'error' or 'fail'
```

### **Replace Text Using `sed`**
```sh
sed -E 's/[0-9]+/NUM/' file.txt  # Replace numbers with 'NUM'
```

---

This guide provides essential knowledge of **file globbing** and **regular expressions** in Linux. 🚀

# **Guide to Working with Different Text Editors in Linux**

This document provides an overview of popular text editors in Linux, their basic usage, and essential commands.

---

## **1. Nano (Beginner-Friendly Editor)**
Nano is a simple and easy-to-use text editor available by default in most Linux distributions.

### **Basic Commands**
| Command | Description |
|---------|-------------|
| `nano filename` | Open or create a file in Nano |
| `CTRL + X` | Exit Nano |
| `CTRL + O` | Save changes |
| `CTRL + R` | Open a file |
| `CTRL + K` | Cut a line |
| `CTRL + U` | Paste a line |
| `CTRL + W` | Search within a file |
| `CTRL + \\` | Find and replace |

---

## **2. Vim (Powerful and Efficient Editor)**
Vim is a highly configurable text editor used for efficient text editing.

### **Modes in Vim**
- **Normal Mode**: Used for navigation and commands (default mode).
- **Insert Mode**: Used for text input (`i` to enter Insert mode).
- **Command Mode**: Used for file operations (`:` followed by a command).

### **Basic Commands**
| Command | Description |
|---------|-------------|
| `vim filename` | Open or create a file in Vim |
| `i` | Enter Insert mode |
| `ESC` | Exit Insert mode |
| `:w` | Save file |
| `:q` | Quit Vim |
| `:wq` or `ZZ` | Save and exit |
| `:q!` | Exit without saving |
| `/search` | Search for text |
| `n` / `N` | Move to next/previous search result |
| `dd` | Delete a line |
| `yy` | Copy a line |
| `p` | Paste content |
| `u` | Undo last change |

---

## **3. Emacs (Extensible and Customizable Editor)**
Emacs is a powerful, extensible editor with a large set of features.

### **Basic Commands**
| Command | Description |
|---------|-------------|
| `emacs filename` | Open or create a file in Emacs |
| `CTRL + X CTRL + S` | Save file |
| `CTRL + X CTRL + C` | Exit Emacs |
| `CTRL + X CTRL + F` | Open a file |
| `CTRL + K` | Cut line |
| `CTRL + Y` | Paste line |
| `CTRL + SPACE` | Start selection |
| `ALT + W` | Copy selection |
| `CTRL + W` | Cut selection |
| `CTRL + /` | Undo |
| `CTRL + S` | Search forward |
| `CTRL + R` | Search backward |

---

## **4. VS Code (Graphical Editor with Extensions)**
Visual Studio Code is a modern, feature-rich editor with support for extensions.

### **Basic Commands**
| Command | Description |
|---------|-------------|
| `code filename` | Open a file in VS Code |
| `CTRL + S` | Save file |
| `CTRL + X` | Cut |
| `CTRL + C` | Copy |
| `CTRL + V` | Paste |
| `CTRL + P` | Quick file open |
| `CTRL + SHIFT + P` | Command palette |
| `CTRL + /` | Toggle comment |
| `CTRL + F` | Find text |
| `CTRL + H` | Replace text |

---

## **5. Sublime Text (Lightweight and Fast Editor)**
Sublime Text is a lightweight and responsive editor with rich features.

### **Basic Commands**
| Command | Description |
|---------|-------------|
| `subl filename` | Open a file in Sublime Text |
| `CTRL + S` | Save file |
| `CTRL + P` | Open file quickly |
| `CTRL + SHIFT + P` | Command palette |
| `CTRL + D` | Select word |
| `CTRL + F` | Find text |
| `CTRL + H` | Replace text |
| `CTRL + L` | Select line |

---

## **6. Micro (Modern Terminal-Based Editor)**
Micro is a modern, easy-to-use terminal-based editor with intuitive shortcuts.

### **Basic Commands**
| Command | Description |
|---------|-------------|
| `micro filename` | Open or create a file in Micro |
| `CTRL + S` | Save file |
| `CTRL + Q` | Quit editor |
| `CTRL + C` | Copy text |
| `CTRL + X` | Cut text |
| `CTRL + V` | Paste text |
| `CTRL + F` | Search text |

---

## **Choosing the Right Editor**
| Editor | Best For |
|--------|----------|
| **Nano** | Beginners who need a simple editor |
| **Vim** | Advanced users who prefer keyboard efficiency |
| **Emacs** | Users who need a fully extensible environment |
| **VS Code** | Developers who want a GUI-based editor with extensions |
| **Sublime Text** | Lightweight and fast code editing |
| **Micro** | A modern alternative to Nano |



# Linux Partitioning, Filesystem, and Swap Management

## 1. Checking and Listing Devices

Before modifying partitions, it’s important to identify available storage devices.

### View System Devices

```sh
lsblk                # Lists all block devices
fdisk -l            # Displays partition table
cat /proc/partitions  # Lists partition details
cat /proc/devices   # Lists character and block devices
```

### Device Naming

- **b** → Block device (e.g., `/dev/sda`, `/dev/sdb`)
- **c** → Character device (e.g., `/dev/tty`, `/dev/random`)
- `/dev/zero` → Provides an infinite stream of zero bytes.

### List Specific Devices

```sh
ls /dev/s??
ls /dev/sd[r]?
```

---

## 2. Understanding Booting, Firmware, and Partition Tables

### Firmware and Bootloaders

- **BIOS (Basic Input/Output System)**: IBM → MBR → Bootloader (GRUB) → Kernel boot.
- **EFI (Extensible Firmware Interface)**: Intel firmware interface.
- **UEFI (Unified Extensible Firmware Interface)**:
  - Requires an **ESP (EFI System Partition)** formatted with FAT.
  - Uses **GPT (GUID Partition Table)** for modern booting.

### Partition Table Types

- **MBR (Master Boot Record)**:
  - Limited to **4 primary partitions** or **3 primary + 1 extended**.
  - Supports disks up to **2TB**.
- **GPT (GUID Partition Table)**:
  - Supports up to **128 partitions**.
  - Works with UEFI booting.
  - Required for disks larger than **2TB**.

---

## 3. Working with Partitions

### Viewing and Managing Partitions

```sh
fdisk -l /dev/sdX    # View partition table of a specific disk
gdisk /dev/sdX       # Manage partitions using GPT
parted /dev/sdX      # Use GNU parted (supports GPT & MBR)
```

### Creating a New Partition Using `fdisk`

```sh
sudo fdisk /dev/sdX
```

- Press **`n`** → Create new partition.
- Choose **`p`** for primary or **`e`** for extended.
- Enter **partition number**.
- Define **sector size** (press **Enter** for defaults).
- Press **`w`** to write changes.

### Resizing Partitions

- If **creating a new partition**, select **yes**.
- If **resizing an existing partition**, ensure you unmount it before resizing.

### Deleting a Partition

```sh
sudo fdisk /dev/sdX
```

- Press **`d`** and choose the partition to delete.
- Press **`w`** to write changes.

---

## 4. Formatting a Partition (Creating a Filesystem)

After creating a partition, format it with a filesystem.

### Common Filesystem Options

```sh
mkfs -t ext4 /dev/sdX1     # Format as ext4
mkfs -t xfs /dev/sdX1      # Format as XFS
mkfs -t ntfs /dev/sdX1     # Format as NTFS
mkfs.vfat -F32 /dev/sdX1   # Format as FAT32
```

---

## 5. Mounting a Partition

### Temporary Mounting

```sh
sudo mkdir /mnt/mydata
sudo mount /dev/sdX1 /mnt/mydata
```

### Persistent Mounting (Auto-Mount on Boot)

Add the following entry to `/etc/fstab`:

```
/dev/sdX1  /mnt/mydata  ext4  defaults  0  2
```

To apply changes:

```sh
sudo mount -a
```

### Unmounting a Partition

```sh
sudo umount /mnt/mydata
```

### Checking Mounts

```sh
lsblk                 # Show mounted block devices
df -h                 # Show disk usage
tail -n1 /proc/mounts # Display last mounted partition
```

---

## 6. Swap Space Management

### Checking Existing Swap

```sh
swapon --show   # Display active swap spaces
free -h         # Show memory usage
```

### Creating Swap Space

#### Method 1: Partition-Based Swap

```sh
sudo mkswap /dev/sdX2
sudo swapon /dev/sdX2
```

Add to `/etc/fstab` for persistence:

```
/dev/sdX2 none swap sw 0 0
```

#### Method 2: File-Based Swap

```sh
sudo fallocate -l 2G /swapfile
sudo chmod 600 /swapfile
sudo mkswap /swapfile
sudo swapon /swapfile
```

Add to `/etc/fstab`:

```
/swapfile none swap sw 0 0
```

### Disabling and Removing Swap

```sh
sudo swapoff -a
sudo rm /swapfile
```

---

## 7. Filesystem Maintenance and Optimization

### Check Disk Usage

```sh
df -h            # Check disk space usage
lsblk            # List block devices
```

### Check and Repair Filesystems

```sh
fsck /dev/sdX1   # Check and repair the filesystem
```

### Manage Filesystem Attributes

```sh
tune2fs -U random /dev/sdX1  # Generate a new UUID
tune2fs -l /dev/sdX1         # Show filesystem details
```

### Free Memory & Cache

```sh
free -h             # Check free memory
sync && echo 3 > /proc/sys/vm/drop_caches  # Clear cache
```

---

## 8. Advanced Partitioning & RAID

### Creating a RAID Array

```sh
mdadm --create --verbose /dev/md0 --level=1 --raid-devices=2 /dev/sdX /dev/sdY
```

### LVM (Logical Volume Manager)

```sh
pvcreate /dev/sdX1
vgcreate my_vg /dev/sdX1
lvcreate -L 10G -n my_lv my_vg
mkfs.ext4 /dev/my_vg/my_lv
mount /dev/my_vg/my_lv /mnt/mydir
```

---

## Conclusion

This guide covers:

- Checking devices and partitions
- Creating, formatting, and mounting partitions
- Setting up and managing swap space
- Filesystem maintenance
- Advanced partitioning with RAID and LVM

This ensures **efficient disk management** and **performance optimization** in Linux.

