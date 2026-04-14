
# 🔐 Secure Coding Review - Task 2

## 📌 Overview
This project demonstrates the difference between a **secure** and an **insecure** login system in Java.

It highlights why storing passwords in plain text is dangerous and how hashing improves security using the **SHA-256 algorithm**.

---

## 📂 Files Included

- `InsecureLogin.java` → Basic login system (NOT secure)
- `SecureLogin.java` → Improved login system with hashing

---

## 🚫 Insecure Login System

### ❌ Description
This version stores and checks passwords in plain text.

### ⚠️ Problems
- Password is hardcoded (`12345`)
- No encryption
- Easily hackable
- No limit on login attempts

---

## ✅ Secure Login System

### 🔐 Description
This version uses **SHA-256 hashing** to secure passwords.

### 🔑 Features
- Password hashing using `MessageDigest`
- No plain-text password storage
- Maximum 3 login attempts
- Account lock after failed attempts

---

## ▶️ How to Run

### Compile
```bash
javac SecureLogin.java
javac InsecureLogin.java
