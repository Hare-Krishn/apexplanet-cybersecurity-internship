# Nmap Scan Report – Task 2

## Network Security & Scanning  
Cybersecurity & Ethical Hacking Internship  
ApexPlanet Software Pvt. Ltd.

---

## Scan Information

- **Target System:** Metasploitable2
- **Target IP Address:** 192.168.15.128
- **Scanning Machine:** Kali Linux
- **Tool Used:** Nmap
- **Nmap Version:** 7.98
- **Scan Date & Time:** Fri Jan 2, 2026

---

## Scan Command Executed

```bash
nmap -sS -sV -O -p- -T4 192.168.15.128
```

---

## Scan Summary

- **Host Status:** Up  
- **Total Ports Scanned:** 65535  
- **Filtered Ports:** 65515  
- **Scan Duration:** 246 seconds  

---

## Open Ports and Services

| Port | Protocol | State | Service |
| ----: | -------- | ----- | ------- |
| 21   | TCP      | Open  | FTP     |
| 22   | TCP      | Open  | SSH     |
| 23   | TCP      | Open  | Telnet  |
| 25   | TCP      | Open  | SMTP    |
| 53   | TCP      | Open  | DNS     |
| 80   | TCP      | Open  | HTTP    |
| 111  | TCP      | Open  | RPC     |
| 139  | TCP      | Open  | NetBIOS |
| 445  | TCP      | Open  | SMB     |
| 3306 | TCP      | Open  | MySQL   |
| 5900 | TCP      | Open  | VNC     |

---

## Closed Ports Detected

| Port | Protocol | Service |
| ----: | -------- | ------- |
| 110  | TCP      | POP3    |
| 113  | TCP      | Ident   |
| 135  | TCP      | MSRPC   |
| 143  | TCP      | IMAP    |
| 443  | TCP      | HTTPS   |
| 993  | TCP      | IMAPS   |
| 1720 | TCP      | H.323   |
| 1723 | TCP      | PPTP    |
| 3389 | TCP      | RDP     |

---

## Service Detection Notes

- Most services were detected as **tcpwrapped**
- Indicates restricted or limited service responses
- Common behavior in deliberately vulnerable systems

---

## Operating System Detection

- **OS Detection Result:** Inconclusive  
- Nmap was unable to accurately identify the operating system  

**Possible reasons:**
- Filtered responses  
- Limited fingerprint data  
- Firewall behavior  

---

## Security Observations

- Multiple insecure and legacy services are exposed
- Plaintext protocols such as **FTP** and **Telnet** are enabled
- **SMB**, **MySQL**, and **VNC** significantly increase the attack surface
- System is intentionally vulnerable and suitable for penetration testing practice

---

## Conclusion

The Nmap scan successfully identified open ports, exposed services, and potential network-level weaknesses on the target system.  
This task demonstrates effective reconnaissance and port scanning techniques as part of **Task 2 – Network Security & Scanning**.

---

## Disclaimer

This scan was conducted in a **controlled lab environment** for educational purposes only.  
No unauthorized or real-world systems were targeted.
