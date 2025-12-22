# Task-1 Notes – Foundation & Environment Setup

## 1. Cybersecurity Basics

### CIA Triad
Confidentiality:
- Prevents unauthorized access to data

Integrity:
- Ensures data is not modified without authorization

Availability:
- Ensures systems and data are accessible when needed

### Common Threat Types
- Phishing – fake emails or websites to steal data
- Malware – malicious software
- DDoS – flooding a service to make it unavailable
- SQL Injection – injecting SQL queries
- Brute Force – guessing passwords
- Ransomware – encrypts data for ransom

### Attack Vectors
- Social Engineering
- Wireless Attacks
- Insider Threats

---

## 2. Lab Environment Setup

### Virtual Machines Used
- Kali Linux – attacker machine
- Metasploitable2 / DVWA – vulnerable target

### Network Configuration
- Host-Only Adapter
- Isolated environment for safe testing

### Verification
- IP addresses checked using `ip a`
- Connectivity tested using `ping`
- Traffic captured using Wireshark

---

## 3. Linux Fundamentals

Linux is widely used in cybersecurity due to its flexibility and security.

### Important Concepts
- File permissions control access
- Root user has full privileges
- Packages are managed using apt and dpkg

---

## 4. Networking Basics

### OSI Model
1. Physical – hardware
2. Data Link – MAC addressing
3. Network – IP addressing
4. Transport – TCP/UDP
5. Session – session management
6. Presentation – encryption
7. Application – user interaction

### TCP/IP Model
- Application
- Transport
- Internet
- Network Interface

### DNS
- Converts domain names to IP addresses

### HTTP vs HTTPS
- HTTP – unencrypted
- HTTPS – encrypted using SSL/TLS

### IP Addressing
- IPv4 example: 192.168.1.1
- Private IP ranges:
  - 10.0.0.0/8
  - 172.16.0.0/12
  - 192.168.0.0/16

### NAT
- Allows private IPs to access public internet

---

## 5. Cryptography Basics

### Encryption
Symmetric Encryption:
- Same key used for encryption and decryption

Asymmetric Encryption:
- Uses public and private keys

### Hashing
- One-way function
- Used for password storage

Examples:
- MD5
- SHA-256

### SSL / TLS
- Secures data in transit
- Used in HTTPS

### OpenSSL
- Used to encrypt and decrypt data
- Provides cryptographic utilities

---

## 6. Tool Familiarization

### Tools Used
- Wireshark – packet analysis
- Nmap – network scanning
- Burp Suite – web proxy testing
- Netcat – network debugging

These tools are essential for ethical hacking and penetration testing.
