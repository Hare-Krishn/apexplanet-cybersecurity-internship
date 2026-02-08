# Web Application Penetration Testing Report – DVWA
## Cybersecurity & Ethical Hacking Internship Capstone Project

**Intern:** Your Name  
**Organization:** ApexPlanet Software Pvt. Ltd.  
**Project:** Web Application Penetration Testing on DVWA  
**Date:** 2026  

---

# 1. Executive Summary
This project demonstrates a complete web application penetration test conducted on DVWA (Damn Vulnerable Web Application) in a controlled lab environment using Kali Linux.

The objective of this capstone project is to identify common web vulnerabilities, exploit them ethically, analyze their impact, and recommend mitigation strategies. An incident response simulation was also performed to demonstrate detection and response to cyber attacks.

This project covers vulnerabilities from OWASP Top 10 including SQL Injection, Cross-Site Scripting (XSS), File Inclusion, and Brute Force attacks.

---

# 2. Objective
- Perform web application penetration testing
- Identify OWASP Top 10 vulnerabilities
- Exploit vulnerabilities in controlled lab
- Suggest mitigation strategies
- Simulate incident response process

---

# 3. Scope
**Target Application:** DVWA (local environment)  
**Attacker Machine:** Kali Linux  
**Testing Type:** Ethical hacking in controlled lab only  
**Out of Scope:** Real-world systems and external networks  

---

# 4. Tools Used
- Kali Linux
- DVWA (Damn Vulnerable Web App)
- Nmap
- Burp Suite
- Hydra
- Browser Developer Tools

---

# 5. Methodology

## Phase 1: Reconnaissance
Identified target system and gathered basic information about running services.

Command used:
```
nmap -sV 127.0.0.1
```

### Screenshot:
(Add Nmap scan screenshot here)

---

## Phase 2: Vulnerability Identification & Exploitation

---

# 6. Vulnerabilities Identified

---

## 6.1 SQL Injection

### Description
SQL Injection vulnerability allows attackers to manipulate database queries and extract sensitive data.

### Payload Used
```
' OR 1=1 #
```

### Result
Successfully bypassed authentication and extracted user credentials.

### Impact
- Unauthorized database access
- Sensitive data exposure
- Account compromise

### Screenshot:
(Add SQL injection screenshot)

### Mitigation
- Use prepared statements
- Input validation
- Parameterized queries
- Web Application Firewall (WAF)

---

## 6.2 Cross-Site Scripting (XSS)

### Description
XSS allows attackers to inject malicious JavaScript into web pages.

### Payload Used
```
<script>alert('XSS')</script>
```

### Result
JavaScript executed in browser showing alert popup.

### Impact
- Session hijacking
- Cookie theft
- Defacement

### Screenshot:
(Add XSS popup screenshot)

### Mitigation
- Input sanitization
- Output encoding
- Content Security Policy (CSP)

---

## 6.3 File Inclusion (LFI)

### Description
Local File Inclusion allows attackers to access sensitive system files.

### Payload Used
```
../../../../etc/passwd
```

### Result
Sensitive system file accessed.

### Impact
- Exposure of system files
- Information disclosure
- Possible remote code execution

### Screenshot:
(Add LFI screenshot)

### Mitigation
- Validate file paths
- Restrict file access
- Disable remote file inclusion

---

## 6.4 Brute Force Attack

### Description
Brute force attack attempts multiple password combinations to gain access.

### Tool Used
Hydra

### Command
```
hydra -l admin -P rockyou.txt 127.0.0.1 http-get-form
```

### Result
Password successfully cracked.

### Impact
- Unauthorized login
- Account compromise

### Screenshot:
(Add Hydra screenshot)

### Mitigation
- Strong passwords
- CAPTCHA
- Rate limiting
- Account lockout policies

---

# 7. Incident Response Simulation

## Incident Scenario
An attacker performed SQL Injection and brute-force attacks to gain unauthorized access.

## Detection
Suspicious requests detected in Apache logs.

Command:
```
sudo tail -f /var/log/apache2/access.log
```

### Screenshot:
(Add log screenshot)

## Containment
- Block attacker IP using firewall
- Disabled vulnerable endpoints

## Eradication
- Fixed SQL injection vulnerability
- Reset user credentials
- Updated input validation

## Recovery
- Restarted web server
- Enabled monitoring
- Verified system integrity

## Lessons Learned
- Implement Web Application Firewall
- Enable continuous monitoring
- Follow secure coding practices
- Conduct regular penetration testing

---

# 8. Conclusion
This capstone project demonstrated practical web application penetration testing skills by identifying and exploiting critical vulnerabilities in DVWA. The project also showcased incident detection and response techniques used by security teams.

The findings highlight the importance of secure coding, regular security testing, and real-time monitoring to protect web applications from cyber threats.

---

# 9. Disclaimer
This project was conducted in a controlled lab environment for educational purposes only. No real systems were harmed or targeted.
