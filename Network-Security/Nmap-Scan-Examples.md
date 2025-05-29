

Nmap Scan Examples
Nmap (Network Mapper) is a powerful open-source tool for network discovery and security auditing. Below are common Nmap scan examples with explanations and sample commands.

1. Basic Host Discovery
bash
nmap 192.168.1.1
Description: Simple scan to check if the host is up and which ports are open.

2. Scan Multiple Hosts
bash
nmap 192.168.1.1 192.168.1.2 192.168.1.3
nmap 192.168.1.1-10
Description: Scan several IP addresses or a range of addresses.

3. Scan an Entire Subnet
bash
nmap 192.168.1.0/24
Description: Scan all 256 hosts in the specified subnet.

4. Service Version Detection
bash
nmap -sV 192.168.1.1
Description: Detects service versions running on open ports.

5. Operating System Detection
bash
nmap -O 192.168.1.1
Description: Attempts to determine the target host’s operating system.

6. Aggressive Scan
bash
nmap -A 192.168.1.1
Description: Performs OS detection, version detection, script scanning, and traceroute.

7. Scan Specific Ports
bash
nmap -p 22,80,443 192.168.1.1
Description: Scan only the specified ports (22, 80, and 443).

8. Stealth (SYN) Scan
bash
nmap -sS 192.168.1.1
Description: Perform a stealth SYN scan (less likely to be logged by the target).

9. UDP Scan
bash
nmap -sU 192.168.1.1
Description: Scan for open UDP ports.

10. Save Scan Results to a File
bash
nmap -oN scan_results.txt 192.168.1.1
Description: Output scan results to a text file for later analysis.

11. Using Nmap Scripting Engine (NSE)
bash
nmap --script vuln 192.168.1.1
Description: Run vulnerability detection scripts against the target.

Example: Aggressive Scan Output
text
nmap -A 192.168.1.1

Starting Nmap 7.93 ( https://nmap.org ) at 2025-05-28 23:30 EDT
Nmap scan report for 192.168.1.1
Host is up (0.0020s latency).
Not shown: 997 closed ports
PORT    STATE SERVICE VERSION
22/tcp  open  ssh     OpenSSH 7.6p1 Ubuntu 4ubuntu0.3 (Ubuntu Linux; protocol 2.0)
80/tcp  open  http    Apache httpd 2.4.29 ((Ubuntu))
443/tcp open  ssl/https
...
OS details: Linux 3.10 - 4.11
