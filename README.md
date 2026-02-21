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
🧪 Lab #2: SQL injection vulnerability allowing login bypass
Status: Solved ✅

Vulnerability Type: Authentication Bypass via SQLi.

The "Back-end" Logic: * The application's login query was likely: SELECT * FROM users WHERE username = '$username' AND password = '$password'

My Exploit Strategy: * I injected administrator'-- into the username field.

How it works: The ' closed the username string, and the -- commented out the rest of the SQL query, including the password check.

This forced the database to return the administrator record without needing a password.

Key Learning: Understanding how the back-end constructs queries is the key to breaking
---
"Don't just find the bug, explain the fix."
