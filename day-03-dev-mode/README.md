# Day 3 - Vault Dev Mode and UI Walkthrough

## What You Will Learn Today

In Day 3, we will explore the HashiCorp Vault UI and understand the main components available inside the Vault dashboard.

By the end of this day, you will understand:

- How to start Vault in Dev Mode
- How to access the Vault UI
- What the Vault dashboard shows
- What Secrets Engines are
- What Access Control means
- What Policies are used for
- What Seal Vault means
- What Operational Tools are
- What Client Count means
- What Configuration section is used for

This is a high-level UI walkthrough.  
We will cover each component in detail in upcoming days.

---

## Start Vault in Dev Mode

To start Vault in Dev Mode, run:

```bash
vault server -dev


- What Configuration section is used for

---

This starts Vault locally.

Vault automatically:

Starts the server
Creates in-memory storage
Initializes Vault
Unseals Vault
Generates Root Token
Starts listener on port 8200
Access Vault UI

Open browser:

http://127.0.0.1:8200

Login using the Root Token generated in the terminal.

Vault Dashboard

The Vault dashboard gives a high-level view of Vault.

Depending on the Vault version and setup, you may see:

Secrets
Access
Resilience and Recovery
Operational Tools
Client Count
Configuration
Vault version
Enabled secrets engines
Quick actions

In Dev Mode, some information may be empty or limited.

In production or HA setup, the dashboard will show more meaningful server and cluster details.

Secrets Engines

Secrets Engines are one of the most important components in Vault.

A secrets engine is responsible for storing, generating, or encrypting secrets.

Examples:

KV secrets engine
Database secrets engine
AWS secrets engine
GCP secrets engine
Azure secrets engine
Transit secrets engine
PKI secrets engine

Each secrets engine has a different purpose.

KV Secrets Engine

KV means Key-Value.

KV secrets engine is used to store static secrets.

Example:

username = admin
password = admin123

It is commonly used to store:

API keys
Passwords
Tokens
Application secrets
Configuration secrets
Access Control

Access Control manages who can log in to Vault and what they are allowed to access.

Inside Access, you may see:

Authentication methods
Policies
Entities
Groups
Leases
MFA
OIDC provider

For now, understand this simply:

Authentication decides who can login.

Policies decide what they can access.

Policies

Policies define permissions in Vault.

Vault is path-based.

Example path:

secret/app/database

A policy can allow or deny actions such as:

read
create
update
delete
list

Policies are one of the most important Vault concepts and will be covered separately.

Resilience and Recovery

This section contains options related to availability, recovery, and sealing.

Some options may be available only in Vault Enterprise.

For beginners, the important concept here is Seal Vault.

Seal Vault

Sealing Vault means locking Vault.

When Vault is sealed:

Vault cannot decrypt secrets
Vault cannot return secret values
Normal secret operations are blocked

In Dev Mode, Vault is automatically initialized and unsealed.

In production, Vault usually starts sealed and must be unsealed before use.

Operational Tools

Operational Tools are used for Vault administrative and security operations.

Examples:

Lookup
Wrapping
Unwrapping
Rewrapping
Token-related operations

These are advanced topics and will be covered later.

Client Count

Client Count shows information about Vault client usage.

It is useful in enterprise or organization-level environments.

For local Dev Mode, this section is not very important.

Configuration

The Configuration section shows server-related information.

Depending on setup, it may include:

Server details
Cluster details
Audit settings
Storage details
License details
Retention settings

In Dev Mode, many values may be empty or limited.

Summary

In Day 3, we learned:

What Dev Mode does
How to access Vault UI
What the Vault dashboard shows
What Secrets Engines are
What Access Control means
What Policies are used for
What Seal Vault means
What Operational Tools are
What Client Count and Configuration sections are used for