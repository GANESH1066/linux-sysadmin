# Module 6: Networking Basics

These are the commands I use to troubleshoot network connectivity issues on a Linux server.

## 1. IP Address Configuration
- `ip a`: Displays all network interfaces and their assigned IP addresses.
- `ip route`: Displays the routing table (shows the default gateway).

## 2. Connectivity Testing
- `ping -c 4 <hostname_or_IP>`: Tests if a remote server is reachable. (Use `-c` to limit the number of pings).
- *Troubleshooting logic:* If `ping 8.8.8.8` works but `ping google.com` fails, it is a DNS issue.

## 3. DNS Resolution
- `dig <domain>`: Queries DNS servers to find the IP address of a domain name.
- `cat /etc/resolv.conf`: Shows which DNS servers the Linux machine is using.

## 4. Open Ports (Crucial)
- `ss -tulnp`: Shows all listening ports and the processes using them.
  - `-t` (TCP), `-u` (UDP), `-l` (Listening), `-n` (Numeric), `-p` (Process).
