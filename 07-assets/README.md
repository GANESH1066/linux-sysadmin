# Module 7: Asset Management

As a sysadmin, I must maintain an accurate inventory of server hardware, OS versions, and licensing.

## 1. OS & Kernel Auditing
- `cat /etc/os-release`: Shows the OS distribution and version.
- `uname -r`: Shows the active Linux kernel version.

## 2. Hardware Inventory
- `lscpu`: Shows detailed CPU architecture and core count.
- `free -h`: Shows total installed RAM.
- `lsblk`: Lists all block devices (hard drives) and their mount points.

## 3. System Summary
- `hostnamectl`: Shows the hostname, OS, kernel, architecture, and virtualization type in one clean output.
