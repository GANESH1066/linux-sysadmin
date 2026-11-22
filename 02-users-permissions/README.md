# Module 2: Users, Groups & Permissions

## 1. Core Files
- `/etc/passwd`: Stores user account information (UID, GID, home directory, shell).
- `/etc/shadow`: Stores encrypted passwords (only accessible by root).
- `/etc/group`: Stores group information.

## 2. User Management Commands
- `useradd -m <username>`: Creates a new user and generates a home directory.
- `passwd <username>`: Sets or changes a user's password.
- `groupadd <groupname>`: Creates a new group.
- `usermod -aG <group> <user>`: Appends a user to a secondary group.
- `id <username>`: Displays the user's UID, GID, and group memberships.
- `userdel -r <username>`: Deletes the user and removes their home directory.

## 3. File Permissions (chmod & chown)
- `chmod`: Changes the permissions of a file. (e.g., `chmod 755 file.sh`).
- `chown`: Changes the owner of a file. (e.g., `sudo chown root:root file.txt`).
- **The Numbers:**
  - 7 = Read + Write + Execute (rwx)
  - 6 = Read + Write (rw-)
  - 5 = Read + Execute (r-x)
  - 4 = Read only (r--)
  - 0 = No permissions (---)
