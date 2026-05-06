# Day 1 - Introduction to Vault & Secrets Management 🔐

---

## 🎯 What You Will Learn Today

* What are secrets?
* Problems with traditional secret management
* What is Vault?
* Why Vault is needed in modern applications

---

## ☁️ Understanding the Problem

In traditional systems, secrets are stored in:

* Source code
* Environment variables
* Configuration files

### ❗ Issues:

* Hard to manage
* Easy to leak
* No proper access control
* Difficult to rotate

---

## 🔄 Traditional vs Vault Approach

### ❌ Without Vault:

Application → Directly uses secrets → Security risk

### ✅ With Vault:

Application → Authenticate → Vault → Get temporary secret

---

## 🔐 What is Vault?

HashiCorp Vault is a tool used to:

* Securely store secrets
* Control access
* Generate dynamic credentials
* Rotate secrets automatically

---

## ⚖️ Why Not Just Use Environment Variables?

| Method        | Problem            |
| ------------- | ------------------ |
| Env Variables | Static & exposed   |
| Config Files  | Hardcoded secrets  |
| Vault         | Secure & dynamic ✅ |

---

## 🧠 Core Concepts (Preview)

* Secrets Engine
* Authentication
* Policies
* Tokens

(Detailed in upcoming days)

---

## 🌍 Real-World Use Cases

* Secure database credentials
* Microservices secret sharing
* API key protection
* Encryption services

---

## 👉 What’s Next?

In Day 2:

* Install Vault
* Run Vault locally
* Explore UI & CLI

---
