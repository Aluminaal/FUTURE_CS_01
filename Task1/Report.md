# Vulnerability Assessment Report

## 1. Introduction
This report presents a basic security assessment conducted on a test web application. The objective is to identify potential vulnerabilities and provide recommendations to improve security.

---

## 2. Target Website
http://testphp.vulnweb.com

---

## 3. Tools Used
- Google Chrome (Browser)
- Manual Inspection

---

## 4. Methodology
The assessment was conducted using basic manual testing techniques, including:
- Observing website behavior
- Inspecting input fields
- Checking protocol security (HTTP/HTTPS)

---

## 5. Vulnerabilities Identified

### 🔴 1. Lack of HTTPS Encryption
- Risk Level: Medium  
- Description:  
  The website uses HTTP instead of HTTPS, meaning data transmitted between the user and server is not encrypted. This exposes sensitive information to interception attacks (Man-in-the-Middle attacks).
  
- Impact:  
  Attackers can intercept login credentials, personal data, or session information.

- Recommendation:  
  Implement HTTPS using an SSL/TLS certificate to ensure secure communication.

---

### 🟡 2. Weak Input Validation
- Risk Level: Medium  
- Description:  
  The website contains input fields (such as search or login forms) that may not properly validate user input. This can allow attackers to inject malicious code (e.g., SQL Injection).

- Impact:  
  Potential unauthorized access to the database or manipulation of data.

- Recommendation:  
  - Implement proper input validation and sanitization  
  - Use prepared statements in database queries  
  - Apply server-side validation

---

## 6. Evidence (Screenshot)

![Website Screenshot](screenshot1.jpg)

---

## 7. Conclusion
The assessment identified key security weaknesses, particularly the absence of HTTPS and potential input validation issues. While the vulnerabilities are basic, they can lead to serious security risks if exploited.

It is recommended that the website implements standard security practices to protect user data and ensure safe operation.
