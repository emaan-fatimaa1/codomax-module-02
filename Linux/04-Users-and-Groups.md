# Linux Users & Groups

### 1. User Types
- **Root User:** Superuser with full administrative privileges (UID 0).
- **Normal User:** Performs regular tasks with limited permissions.
- **System User:** Used by system services and background processes.

### 2. Important Concepts
- **UID:** Unique User ID.
- **GID:** Group ID.
- **Primary Group:** Main group assigned to a user.
- **Secondary Group:** Additional groups a user belongs to.

### 3. User Management Commands

| Command | Purpose |
|---|---|
| `whoami` | Show current username |
| `id` | Show user ID and groups |
| `who` | Show logged-in users |
| `sudo useradd -m username` | Create user with home directory |
| `sudo passwd username` | Set/change password |
| `sudo usermod -l new old` | Change username |
| `sudo usermod -L username` | Lock password |
| `sudo usermod -U username` | Unlock password |
| `sudo userdel -r username` | Delete user and home directory |

### 4. Group Management Commands

| Command | Purpose |
|---|---|
| `groups` | Show user's groups |
| `sudo groupadd groupname` | Create group |
| `sudo groupmod -n new old` | Rename group |
| `sudo groupdel groupname` | Delete group |
| `sudo usermod -aG groupname username` | Add user to supplementary group |
| `getent group groupname` | View group information |

### 5. Important Linux Files

- `/etc/passwd` – Stores basic user account information.
- `/etc/shadow` – Stores password hashes and password-related information.
- `/etc/group` – Stores group information.

**Remember:** Use `usermod -aG` to add a user to a supplementary group without replacing existing supplementary group memberships.
