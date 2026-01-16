# Attack Scenarios and Mitigation Notes  
## Task 3 – Web Application Security

This document explains **how common web attacks are performed** and **how they can be prevented**, based on practical testing in a controlled DVWA lab environment.

---

## 1. SQL Injection (SQLi)

### Attack Scenario
1. An attacker identifies an input field that interacts with the backend database.
2. Instead of providing valid input, the attacker injects malicious SQL code.
3. The application directly concatenates user input into the SQL query.
4. The database executes the attacker-controlled query.
5. Sensitive information such as usernames and passwords is returned.

### Mitigation Notes
- Do not concatenate user input directly into SQL queries.
- Use **prepared statements (parameterized queries)** to separate SQL logic from user input.
- Apply server-side input validation and least-privilege database access.
- These measures ensure injected SQL code is treated as data, not executable commands.

---

## 2. Cross-Site Scripting (XSS)

### Attack Scenario
1. An attacker injects malicious JavaScript through form inputs or URL parameters.
2. The application fails to validate or sanitize the input.
3. The malicious script is stored in the database (Stored XSS) or reflected back in the response (Reflected XSS).
4. When a victim accesses the affected page, the script executes in the victim’s browser.

### Mitigation Notes
- Validate and sanitize all user input.
- Encode output before rendering it in the browser.
- Implement **Content Security Policy (CSP)** to restrict script execution.
- These controls prevent execution of unauthorized scripts in the client’s browser.

---

## 3. Cross-Site Request Forgery (CSRF)

### Attack Scenario
1. A victim logs into the web application and maintains an active session.
2. The attacker tricks the victim into visiting a malicious webpage.
3. The browser automatically sends an authenticated request to the target application.
4. The application processes the request without verifying its origin.
5. Unauthorized actions (such as password changes) are performed.

### Mitigation Notes
- Implement **CSRF tokens** for all state-changing requests.
- Validate tokens on the server before processing requests.
- Avoid using GET requests for sensitive operations.
- These protections ensure that only legitimate user-initiated requests are accepted.

---

## Conclusion
Understanding both the **attack techniques** and the **corresponding mitigations** is essential for building secure web applications. Implementing secure coding practices and proper validation mechanisms significantly reduces the risk of exploitation.
