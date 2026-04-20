# Vulnerability Assessment Report

## 1. Objective
The objective of this task is to perform a basic security assessment on a vulnerable web application and identify potential security weaknesses. The goal is to understand how vulnerabilities can be discovered and how they impact system security.

---

## 2. Target Application
OWASP Juice Shop  
https://juice-shop.herokuapp.com

---

## 3. Tools Used
- Nmap (Network Scanning)
- OWASP ZAP (Web Application Security Scanner)
- Mozilla Firefox (Manual Testing)

---

## 4. Methodology

### Step 1: Reconnaissance
- Accessed the application using a web browser
- Observed application structure, login system, and input fields

### Step 2: Network Scanning (Nmap)
- Performed a basic scan to identify open ports and services
- Verified that the web application is accessible over HTTP/HTTPS

### Step 3: Automated Scanning (OWASP ZAP)
- Used ZAP to scan the application for common vulnerabilities
- Identified alerts related to input validation and security misconfigurations

### Step 4: Manual Testing
- Tested input fields manually for unusual behavior
- Checked login and search functionalities for possible weaknesses

---

## 5. Vulnerabilities Identified

### 1. Cross-Site Scripting (XSS)
- Risk Level: Medium
- Description:
  Input fields may allow malicious scripts to be injected and executed in the browser.
- Impact:
  Attackers can steal session data or perform actions on behalf of users.
- Recommendation:
  Implement input validation and output encoding.

---

### 2. Security Misconfiguration
- Risk Level: Medium
- Description:
  The application exposes certain unnecessary information and lacks strict security configurations.
- Impact:
  Attackers can gather information about the system and exploit weaknesses.
- Recommendation:
  Disable unnecessary features and configure secure headers.

---

### 3. Weak Authentication Mechanism
- Risk Level: High
- Description:
  The authentication system may allow weak passwords or improper validation.
- Impact:
  Unauthorized users can gain access to accounts.
- Recommendation:
  Enforce strong password policies and proper authentication controls.

---

## 6. Evidence (Screenshots)
- Nmap scan results
- OWASP ZAP scan alerts
- Browser testing screenshots

---

## 7. Conclusion
The OWASP Juice Shop application contains multiple vulnerabilities intentionally designed for educational purposes. This assessment provided practical experience in identifying common web security issues using both automated and manual testing techniques.

---

## 8. Learning Outcome
- Gained hands-on experience with Nmap and OWASP ZAP
- Understood common web vulnerabilities like XSS and authentication flaws
- Learned how to analyze and document security findings professionally
