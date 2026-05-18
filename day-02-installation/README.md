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

## Vault Installation

Vault is distributed as a binary.

That means we download the Vault executable and configure it so that we can run Vault commands from the terminal.

Installing Vault on Windows:

Steps:

Download Vault from the official HashiCorp website.
https://developer.hashicorp.com/vault/install#windows
Extract the ZIP file.
Copy the folder path where vault.exe is available.
Add that folder path to the system PATH environment variable.
Open a new terminal.

After installation, the following command should work:

```bash
vault --version