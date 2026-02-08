# Penetration Testing Methodology

## 1. Planning & Scope
Target: DVWA (local lab)
Attacker: Kali Linux
Testing type: Controlled ethical hacking lab

## 2. Reconnaissance
- Identified target IP address
- Checked running services using Nmap

## 3. Scanning
Used Nmap to detect:
- Open ports
- Running services
- Web server details

Command used:
nmap -sV 127.0.0.1

## 4. Exploitation

### SQL Injection
- Bypassed login using SQL payload
- Extracted user credentials

### Cross-Site Scripting (XSS)
- Injected JavaScript payload
- Demonstrated stored XSS popup

### File Inclusion
- Accessed sensitive system files
- Demonstrated Local File Inclusion

### Brute Force
- Used Hydra to brute-force login credentials

## 5. Post Exploitation
- Verified access gained
- Documented vulnerabilities

## 6. Reporting
All findings documented with:
- Screenshots
- Impact
- Mitigation strategies
