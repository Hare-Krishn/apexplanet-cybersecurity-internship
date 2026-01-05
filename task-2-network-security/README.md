# Network Security & Scanning  
**TASK – 2**  
**Timeline:** Days 13–24  

🌐 **Website:** www.apexplanet.in  

---

## Objective

Learn and apply **reconnaissance, network scanning, vulnerability assessment, network traffic analysis**, and **basic firewall configuration**, including attack simulation, in a controlled lab environment.

---

## Reconnaissance

### Passive Reconnaissance
- Whois
- Nslookup
- Google Dorking
- Shodan

### Active Reconnaissance
- Ping sweep
- Banner grabbing

---

## Port & Service Scanning

### Scanning Techniques
- TCP SYN scan (`-sS`)
- UDP scan (`-sU`)
- Service version detection (`-sV`)
- Operating system detection (`-O`)

### Tool Used
- **Nmap**

### Output
- Detailed scan reports created for target systems

---

## Vulnerability Scanning

### Vulnerability Assessment
- Setup and configuration of **OpenVAS** or **Nessus Essentials**
- Vulnerability scan performed on **Metasploitable2** test virtual machine
- Vulnerabilities analyzed and categorized based on severity:
  - Critical
  - High
  - Medium
  - Low

---

## Packet Analysis with Wireshark

### Traffic Captured
- HTTP traffic
- FTP traffic
- DNS traffic

### Analysis Performed
- Inspection of unencrypted HTTP and FTP traffic
- Filtering and identification of credentials from unencrypted FTP sessions
- Analysis of ICMP and TCP packets

### SYN Flood Attack Simulation
- SYN flood attack simulated using **hping3**
- High volume of TCP SYN packets generated toward the target
- Packet behavior observed and analyzed in **Wireshark**
- Impact of excessive SYN requests on network traffic examined

---

## Firewall Basics

### Firewall Configuration
- Creation of simple **iptables** rules
- Allowing and denying specific ports
- Demonstration of blocking a port scan attempt
- Verification of firewall effectiveness using Nmap scans

---

## Tools Used

- **Nmap** – Network and port scanning
- **OpenVAS / Nessus Essentials** – Vulnerability scanning
- **Wireshark** – Packet capture and analysis
- **hping3** – SYN flood attack simulation
- **iptables** – Firewall configuration
- **Kali Linux** – Attacker machine
- **Metasploitable2** – Target test machine

---

## Deliverables

- **Nmap Scan Report**
- **OpenVAS / Nessus Vulnerability Report**
- **GitHub Repository**
  - Detailed scan analysis
  - Reconnaissance documentation
  - Packet analysis with Wireshark
  - SYN flood simulation analysis
  - Firewall rule demonstration
- **5-Minute Demo Video**
  - Scan execution
  - Vulnerability findings
  - SYN flood observation
  - Firewall blocking demonstration

---

## Outcome

This task developed hands-on skills in **network reconnaissance, scanning, vulnerability assessment, traffic analysis, attack simulation, and firewall configuration**, strengthening core network security knowledge.

