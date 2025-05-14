# 📧 Email Enumeration via Verbose Login Feedback

This script automates the process of **enumerating valid email addresses** by interacting with a vulnerable web application's verbose login functionality. It checks which email addresses exist based on server response messages.

---

## 🚀 How It Works

The script sends a `POST` request to a login endpoint, providing a **test password** for each email.

It analyzes the server's **JSON response** to distinguish between:

- ✅ **Valid emails** — When the response indicates an incorrect password but **not** a non-existent email.
- ❌ **Invalid emails** — When the server clearly states the **email does not exist**.

> ⚠️ This technique relies on **verbose error messages** from the server — a common misconfiguration in web applications.

---
