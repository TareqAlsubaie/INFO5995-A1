# INFO5995 Assignment 1  
**AI-Assisted Cryptographic Vulnerability Discovery**

---

## 📌 Overview
This project analyses an Android application package (`a1_case1.apk`) to identify and evaluate a **security vulnerability related to randomness and authentication**.

The focus of this assignment is to:
- Model the system and threat environment  
- Identify a cryptographic/randomness vulnerability  
- Demonstrate how it can be exploited  
- Propose and justify a secure fix  

---

## 🧠 Key Findings
- The application generates session tokens using `java.util.Random`
- This is **not cryptographically secure**
- Tokens can be **predicted or reproduced**
- This enables **session manipulation and impersonation attacks**

---

## ⚠️ Vulnerability Summary
| Component | Issue |
|----------|------|
| Login class | Weak randomness (`java.util.Random`) |
| Session token | Predictable |
| Storage | Stored in SharedPreferences |
| Impact | Authentication bypass / impersonation |

---

## 🛠️ Fix / Mitigation
The vulnerability is fixed by replacing:
```java
java.util.Random