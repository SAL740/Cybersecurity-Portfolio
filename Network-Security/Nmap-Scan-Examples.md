
# Nmap Scan Examples

**Nmap** (Network Mapper) is a powerful open-source tool for network discovery and security auditing. Below are common Nmap scan examples with explanations and sample commands.


## 1. Basic Host Discovery
nmap 111.111.1.1

**Description:** Simple scan to check if the host is up and which ports are open.



## 2. Scan Multiple Hosts
nmap 111.111.1.1 111.111.1.2 111.199.1.3
nmap 111.199.1.1-10




**Description:** Scan several IP addresses or a range of addresses.



## 3. Scan an Entire Subnet
nmap 111.111.1.0/24


**Description:** Scan all 256 hosts in the specified subnet.



## 4. Service Version Detection

nmap -sV 111.111.1.1


**Description:** Detects service versions running on open ports.



## 5. Operating System Detection

nmap -O 111.111.1.1


**Description:** Attempts to determine the target host’s operating system.



## 6. Aggressive Scan

nmap -A 111.111.1.11



**Description:** Performs OS detection, version detection, script scanning, and traceroute.



## 7. Scan Specific Ports

nmap -p 45,25,777 111.111.1.1



**Description:** Scan only the specified ports (45, 25, and 777).



## 8. Stealth (SYN) Scan
nmap -sS 111.111.1.1



**Description:** Perform a stealth SYN scan (less likely to be logged by the target).



## 9. UDP Scan

nmap -sU 111.111.1.1


**Description:** Scan for open UDP ports.



## 10. Save Scan Results to a File

nmap -oN scan_results.txt 111.111.1.1



**Description:** Output scan results to a text file for later analysis.



## 11. Using Nmap Scripting Engine (NSE)

nmap --script vuln 111.111.1.1




**Description:** Run vulnerability detection scripts against the target.



## Example: Aggressive Scan Output
nmap -A 111.111.1.1

Starting Nmap 7.93 ( https://nmap.org ) at 2025-05-28 23:30 EDT
Nmap scan report for 111.111.1.1
Host is up (0.0020s latency).
Not shown: 997 closed ports
PORT STATE SERVICE VERSION
22/tcp open ssh OpenSSH 7.6p1 Ubuntu 4ubuntu0.3 (Ubuntu Linux; protocol 2.0)
80/tcp open http Apache httpd 2.4.29 ((Ubuntu))
443/tcp open ssl/http




## References

- [Nmap Official Documentation](https://nmap.org/book/man.html)
- [Nmap Cheat Sheet (SANS)](https://www.sans.org/blog/nmap-cheat-sheet/)
- [Nmap Scripts Documentation](https://nmap.org/nsedoc/)



**Note:**  
Always ensure you have permission before scanning any network or system.













