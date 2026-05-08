# Day 2 - Install HashiCorp Vault Locally

## What You Will Learn Today

In Day 2, we will install HashiCorp Vault and run Vault locally in Dev Mode.

By the end of this day, you will understand:

- How to download Vault
- How to add Vault to system PATH
- How to verify Vault installation
- How to start Vault in Dev Mode
- What Root Token means
- What Vault Address means
- How to access Vault UI
- Why Dev Mode is not for production

---

## Quick Recap from Day 1

In Day 1, we learned that secrets are sensitive values such as:

- Database passwords
- API keys
- Tokens
- Certificates
- Cloud credentials

We also understood that storing secrets directly in code, config files, or environment variables creates security risks.

Vault solves this problem by providing centralized secrets management.

---

## What are We Doing Today?

Today we are not going deep into policies, authentication methods, or secrets engines.

The goal is simple:

```text
Install Vault
     |
     v
Start Vault locally
     |
     v
Login to Vault UI
     |
     v
Prepare for hands-on practice