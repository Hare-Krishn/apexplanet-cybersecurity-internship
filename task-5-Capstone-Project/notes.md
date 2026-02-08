# DVWA Pentesting Notes

## Objective
Perform web application penetration testing on DVWA and identify vulnerabilities based on OWASP Top 10.

## Environment
Attacker Machine: Kali Linux  
Target Application: DVWA (localhost)  
Testing Type: Controlled lab testing  

## Reconnaissance
Used Nmap to scan target system and identify open ports and running services.

## Vulnerabilities Identified

### 1. SQL Injection
Allowed bypassing authentication and extracting user data.

Impact:
Unauthorized database access and data leakage.

Mitigation:
Use prepared statements and input validation.

### 2. Cross Site Scripting (XSS)
Injected JavaScript executed in browser.

Impact:
Session hijacking and cookie theft.

Mitigation:
Input sanitization and CSP headers.

### 3. File Inclusion
Accessed sensitive system files.

Impact:
Exposure of system configuration and credentials.

Mitigation:
Restrict file paths and validate input.

### 4. Brute Force Attack
Used Hydra to crack login credentials.

Impact:
Unauthorized account access.

Mitigation:
Strong passwords, CAPTCHA, rate limiting.

## Incident Response Simulation

Detection:
Suspicious logs detected in Apache access log.

Containment:
Blocked attacker IP and disabled vulnerable endpoints.

Eradication:
Patched vulnerabilities and reset passwords.

Recovery:
Restarted services and enabled monitoring.

## Conclusion
This project demonstrated real-world web application vulnerabilities and how security teams detect and respond to attacks.
