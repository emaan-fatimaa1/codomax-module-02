# SSH (Secure Shell)

## 1. What is SSH?
SSH (Secure Shell) is a network protocol used to securely connect to and manage a remote computer/server over a network.

**Example:** A cloud engineer can access an AWS Linux server from their own computer using SSH.

## 2. Why is SSH Important?
- Secure remote access to servers.
- Allows administrators to manage remote Linux systems.
- Encrypts communication between two devices.
- Commonly used in Cloud Computing and DevOps.

## 3. Important SSH Commands

| Command | Purpose |
|---|---|
| `ssh username@IP` | Connect to a remote server |
| `ssh-keygen` | Generate SSH key pair |
| `ssh-add` | Add a private key to SSH agent |
| `ssh -i key.pem username@IP` | Connect using a specific private key |
| `exit` | Disconnect from SSH session |

## 4. SSH Key Authentication

SSH supports key-based authentication using two keys:

- **Public Key:** Shared with the remote server.
- **Private Key:** Kept secret on your local computer.

Both keys work together to authenticate a user securely.

### Generate SSH Keys
```bash
ssh-keygen
```

This generates:
- `id_rsa` – Private Key
- `id_rsa.pub` – Public Key

**Important:** Never share your private key with anyone.

## 5. SSH in Cloud & DevOps

SSH is commonly used to:
- Access AWS EC2 Linux instances.
- Manage remote servers.
- Deploy applications.
- Perform server administration.
- Troubleshoot Linux servers.

## Conclusion
SSH is an essential tool for Linux system administration, Cloud Computing, and DevOps because it provides secure remote access to servers.
