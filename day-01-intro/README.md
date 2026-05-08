

# Day 1 - Introduction to Vault and Secrets Management

## What You Will Learn Today

In Day 1, we will understand why secrets management is important and how HashiCorp Vault helps solve real-world security problems.

By the end of this day, you will understand:

- What secrets are
- Why storing secrets directly in code is risky
- Problems with traditional secret management
- What HashiCorp Vault is
- Why Vault is useful in modern DevOps environments
- Basic Vault flow
- Real-world Vault use cases

---

## What are Secrets?

Secrets are sensitive values used by applications, systems, and users to authenticate or connect with other services.

Examples of secrets:

- Database username and password
- API keys
- Access tokens
- SSH keys
- TLS certificates
- Cloud credentials
- Application passwords

These values should never be exposed publicly.

---

## The Problem Without Vault

In many real-world applications, secrets are stored in unsafe places such as:

- Source code
- `.env` files
- Configuration files
- CI/CD pipeline variables without proper control
- Shared documents
- Local machines
- Plain Kubernetes secrets without additional protection

This creates serious security risks.

---

## Common Risks

If secrets are not managed properly, the following problems can happen:

- Secrets can be leaked through GitHub repositories
- Developers may accidentally expose credentials
- Old credentials may never get rotated
- Multiple teams may share the same credentials
- There may be no clear audit trail
- Access control becomes difficult
- Production credentials may be reused in lower environments

---

## Traditional Approach vs Vault Approach

### Without Vault

```text
Application
     |
     | Directly reads password/API key
     v
Config file / Env variable / Source code
     |
     v
Security Risk
```

### With Vault
```text
User / Application
        |
        | Login using auth method
        v
HashiCorp Vault
        |
        | Check policy
        v
Secrets Engine
        |
        | Return secret if allowed
        v
User / Application
```