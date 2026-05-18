# HashiCorp Vault Zero to Hero

This repository is a structured 21-day learning path to understand HashiCorp Vault from basics to real-world DevOps and production use cases.

The goal of this repository is to help learners understand Vault even if they directly read the documentation without watching the complete video series.

Each day contains beginner-friendly theory, practical context, and important concepts required to build a strong understanding of Vault.

---

## What is HashiCorp Vault?

HashiCorp Vault is a secrets management and data protection tool used to securely store, access, generate, and manage sensitive information.

Examples of secrets:

- Database passwords
- API keys
- Access tokens
- TLS certificates
- SSH keys
- Cloud credentials
- Application credentials

Vault helps DevOps, cloud, platform, and security teams manage secrets in a centralized and controlled way.

---

## Why Learn Vault?

In real-world projects, secrets are often stored in unsafe places such as:

- Source code
- `.env` files
- Configuration files
- CI/CD variables
- Shared documents
- Local machines
- Kubernetes secrets without additional protection

This creates security risks.

Vault helps solve these problems by providing:

- Centralized secrets management
- Authentication and authorization
- Policy-based access control
- Dynamic secrets
- Secret leasing and TTL
- Secret rotation
- Audit logging
- Encryption as a service
- Kubernetes and cloud integration
- Production-ready secret management

---

## Learning Path

## Day 1: Introduction to Vault and Secrets Management

- What are secrets?
- Why secrets management is important
- Problems with hardcoded secrets
- Traditional secret storage vs Vault
- Vault vs cloud secret managers
- Real-world Vault use cases

## Day 2: Installing Vault Locally

- Download and install Vault
- Configure Vault in system PATH
- Verify Vault installation
- Start Vault in Dev Mode
- Understand Root Token and Vault Address
- Access Vault UI

## Day 3: Vault Dev Mode and UI Walkthrough

- What is Vault Dev Mode?
- Why Dev Mode is used for learning
- Vault UI overview
- Secrets Engines overview
- Access Control overview
- Policies overview
- Operational Tools overview

## Day 4: Vault Core Concepts

- Secrets
- Secrets Engines
- Auth Methods
- Tokens
- Policies
- Paths
- Capabilities

## Day 5: KV Secrets Engine

- What is KV secrets engine?
- KV v1 vs KV v2 overview
- Store static secrets
- Read secrets
- Update secrets
- Delete secrets

## Day 6: Vault Authentication Methods

- What are authentication methods?
- Token authentication
- Userpass authentication
- AppRole authentication overview
- Kubernetes authentication overview
- Choosing the right auth method

## Day 7: Vault Policies

- What are Vault policies?
- Path-based access control
- Policy capabilities
- Read/write/list/delete permissions
- Policy examples
- Best practices

## Day 8: KV Version 2

- What is KV v2?
- Secret versioning
- Metadata
- Soft delete
- Destroy secret versions
- Use cases of versioned secrets

## Day 9: Dynamic Secrets

- Static secrets vs dynamic secrets
- Why dynamic secrets are important
- Database secrets engine overview
- Temporary credentials
- TTL and expiry

## Day 10: Leasing and TTL

- What is a lease?
- What is TTL?
- Renewing leases
- Revoking leases
- Why leases are important for security

## Day 11: Vault CLI and API

- Vault CLI basics
- Vault API overview
- CLI vs API
- Authentication using CLI/API
- Reading and writing secrets using API

## Day 12: Application Integration

- Why applications need Vault
- How applications authenticate to Vault
- Fetching secrets at runtime
- Node.js / Java / Python integration overview
- Avoiding hardcoded application secrets

## Day 13: Secret Injection

- What is secret injection?
- Environment variable injection
- File-based secret injection
- Pros and cons
- Best practices

## Day 14: Vault Agent

- What is Vault Agent?
- Auto-auth overview
- Template rendering
- Secret caching
- Vault Agent use cases

## Day 15: Vault Agent Auto-Auth

- What is Auto-Auth?
- AppRole Auto-Auth
- Kubernetes Auto-Auth
- Sink files
- Runtime secret delivery

## Day 16: Transit Secrets Engine

- What is Transit engine?
- Encryption as a service
- Encrypt and decrypt data
- Key management
- Real-world encryption use cases

## Day 17: Kubernetes Authentication

- Vault and Kubernetes integration
- Kubernetes auth method
- Service accounts
- Vault roles
- Pod authentication flow

## Day 18: Vault with Docker

- Running Vault with Docker
- Docker Compose setup
- Persistent storage overview
- Local production-like setup
- Common Docker-based Vault use cases

## Day 19: Vault High Availability Basics

- Why HA is required
- Vault storage backend overview
- Raft integrated storage
- Leader and standby nodes
- HA architecture basics

## Day 20: Vault Security Best Practices

- Root token handling
- Least privilege policies
- Audit logging
- TLS usage
- Secret rotation
- Avoiding common mistakes

## Day 21: Real-World Vault Architecture

- Production Vault architecture
- Vault with Kubernetes
- Vault with CI/CD
- Vault with cloud KMS
- HA and backup strategy
- Final recap

---

## Repository Structure

```text
Hashicorp-Vault-Zero-to-Hero/
├── README.md
├── Day-01/
│   └── README.md
├── Day-02/
│   └── README.md
├── Day-03/
│   └── README.md
├── Day-04/
│   └── README.md
...
└── Day-21/
    └── README.md