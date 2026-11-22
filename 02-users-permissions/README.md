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
