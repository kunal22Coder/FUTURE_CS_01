# Cyber Security Internship Task 1

## Vulnerability Assessment Report

### Prepared By
Prashant Khare

---

## Objective
The objective of this task is to perform a passive vulnerability assessment on a public demo website using ethical and read-only testing techniques.

---

## Target Website
https://demo.testfire.net

---

## Scope
This assessment included:

- Passive vulnerability scanning
- Header analysis
- Cookie inspection
- Configuration review

The following activities were NOT performed:

- Exploitation
- Brute force attacks
- Denial of Service (DoS)
- Login bypass attempts

---

## Tools Used

- Nmap
- OWASP ZAP
- Browser DevTools
- GitHub

---

## Findings

### 1. Content Security Policy (CSP) Header Not Set
Risk Level: Medium

The application does not implement a Content Security Policy header, increasing the risk of Cross-Site Scripting (XSS) attacks.

---

### 2. Missing Anti-clickjacking Header
Risk Level: Medium

The application does not protect against clickjacking attacks.

---

### 3. Cookie without SameSite Attribute
Risk Level: Low

Cookies are not configured with the SameSite attribute.

---

### 4. Server Version Information Disclosure
Risk Level: Low

The server exposes version-related information through HTTP headers.

---

### 5. Strict-Transport-Security Header Not Set
Risk Level: Medium

The application does not enforce secure HTTPS communication.

---

## Recommendations

- Implement Content Security Policy headers
- Configure secure cookie attributes
- Hide unnecessary server information
- Enable HSTS protection
- Improve HTTP security headers

---

## Evidence

Screenshots and scan outputs are available in the repository folders.

---

## Disclaimer

This project was performed for educational purposes only using passive and ethical security testing methods.
