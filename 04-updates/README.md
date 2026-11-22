# Module 4: Updates & Patching

Applying updates is critical for server security. I use the `dnf` package manager on Rocky Linux/RHEL.

## 1. Checking for Updates
- `sudo dnf check-update`: Lists all available security and software updates without installing them.

## 2. Applying Updates
- `sudo dnf update -y`: Downloads and installs all available updates automatically.
- *Note: After a kernel update, the server must be rebooted for the new kernel to take effect.*

## 3. Auditing Updates
- `sudo dnf history`: Shows a log of all past package installations, updates, and removals.
- `sudo dnf history undo <ID>`: Reverts a specific transaction if an update breaks a service.
