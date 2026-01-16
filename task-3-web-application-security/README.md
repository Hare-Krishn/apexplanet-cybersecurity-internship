# Web Application Security  
**TASK – 3**  
**Timeline: Days 25–36**

🌐 **Website:** www.apexplanet.in

---

## Objective
Learn and apply web application security testing techniques by identifying,
exploiting, and mitigating **OWASP Top 10 vulnerabilities** in a controlled lab
environment.

---

## Vulnerabilities Tested

### SQL Injection (SQLi)
- Exploitation of vulnerable input fields to manipulate backend SQL queries
- Extraction of sensitive data such as usernames and passwords
- Understanding the impact of improper input handling

---

### Cross-Site Scripting (XSS)

**Stored XSS**
- Injection of malicious JavaScript stored in the database
- Script execution for all users accessing the affected page

**Reflected XSS**
- Injection of malicious scripts via URL parameters
- Immediate execution in the victim’s browser

---

### Cross-Site Request Forgery (CSRF)
- Forged requests created to perform unauthorized actions
- Password change performed without user consent
- Demonstration of attack execution using malicious HTML

---

## Web Application Attacks

### File Inclusion Attacks

**Local File Inclusion (LFI)**
- Reading sensitive server files using path traversal techniques

**Remote File Inclusion (RFI)**
- Execution of malicious remote code in insecure configurations

---

## Advanced Testing Techniques

### Burp Suite
- Interception and modification of login requests
- Fuzzing of parameters using Intruder
- Analysis of server responses for vulnerabilities

---

### Web Security Headers
- Analysis of HTTP security headers using `securityheaders.com`
- Identification of missing security headers
- Implementation of recommended headers in Apache configuration

---

## Mitigation Techniques
- Prepared statements for SQL Injection prevention
- Input validation and output encoding for XSS mitigation
- Content Security Policy (CSP) implementation
- CSRF token-based request validation
- Secure server-side configuration for file inclusion prevention
- Proper HTTP security headers configuration

---

## Tools Used
- **Kali Linux** – Attacker and testing environment  
- **DVWA (Damn Vulnerable Web Application)** – Vulnerable web application  
- **Burp Suite** – Web request interception and fuzzing  
- **Apache Web Server** – Web server configuration  
- **securityheaders.com** – HTTP header analysis  

---

## Deliverables
- **Security Testing Report**
  - SQL Injection, XSS, and CSRF testing results
- **Attack Scenarios and Mitigation Notes**
  - Explanation of attack flow and prevention techniques
- **GitHub Repository**
  - Organized documentation and screenshots
- **8-Minute Demo Video**
  - Vulnerability exploitation
  - Impact explanation
  - Mitigation implementation
  - Re-testing to verify fixes

---

## Outcome
This task provided hands-on experience in exploiting and mitigating common web
application vulnerabilities, strengthening practical understanding of secure
coding practices and web application defense mechanisms.
