# 🚀 My Cyber Security Journey

Welcome to my security research lab! I am a **1st Year Cyber Security Engineering Student** with a background in **Front-end & Back-end Development**. 

### 🎯 My Goal
Moving beyond the "script kiddie" mindset to understand the deep engineering behind web vulnerabilities and how to build secure-by-design systems.

### 🛡️ Current Focus
* **Platform:** PortSwigger Web Security Academy.
* **Tools:** Burp Suite Professional/Community.
* **Vulnerabilities:** SQL Injection (Current), Authentication, and Access Control.

### 🛠️ Projects & Writeups
* [Lab #1: SQL injection in WHERE clause] - Done ✅
* [Secure Coding Example #1: How to prevent XSS] - Done ✅
### 🛡️ Practical Security Research (PortSwigger Academy)

#### 🧪 Lab #1: SQL injection in WHERE clause (Retrieving hidden data)
* **Status:** `Solved ✅`
* **Vulnerability Type:** SQL Injection (SQLi).
* **Back-end Logic Analysis:** The application filters products using a SQL query similar to: 
    `SELECT * FROM products WHERE category = 'Gifts' AND released = 1`
* **Exploitation Technique:** By leveraging my **Back-end knowledge**, I injected a comment indicator `--` to terminate the query early, effectively bypassing the `AND released = 1` condition.
* **Outcome:** Successfully retrieved unreleased products, proving the impact of improper input sanitization. 

---
"Don't just find the bug, explain the fix."
