# Module 3: Server Monitoring

These are the commands I use to check the health of a Linux server.

## 1. Disk Space
- `df -h`: Shows how much disk space is used on all mounted filesystems. If a disk hits 100%, services will crash.

## 2. Memory (RAM)
- `free -h`: Shows total, used, and free RAM. 

## 3. System Load & Uptime
- `uptime`: Shows how long the server has been running and the load average (over 1 min, 5 min, 15 min).

## 4. Running Processes
- `top`: Shows a real-time, live view of all running processes, CPU usage, and memory usage. (Press 'q' to quit).
