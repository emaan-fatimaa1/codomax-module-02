# Linux File Permissions

## 1. Introduction
Linux permissions control who can read, write, or execute files and directories.

## 2. Permission Types

| Permission | Symbol | Meaning |
|---|---|---|
| Read | r | Read contents |
| Write | w | Modify contents |
| Execute | x | Execute files |

## 3. Permission Categories

- `u` – Owner
- `g` – Group
- `o` – Others
- `a` – All users

## 4. Important Commands

| Command | Purpose |
|---|---|
| `ls -l` | Check permissions |
| `chmod` | Change permissions |
| `chown` | Change file owner |
| `chgrp` | Change group |
| `umask` | Set default permission restrictions |
| `stat` | View detailed file information |
| `id` | Check user and group IDs |

## 5. chmod Examples

**Symbolic Method:**
```bash
chmod u+x file.txt
chmod g+w file.txt
chmod o-r file.txt
```

**Numeric Method:**

| Number | Permission |
|---|---|
| 755 | rwxr-xr-x |
| 644 | rw-r--r-- |
| 600 | rw------- |

Permission values: Read = 4, Write = 2, Execute = 1.

## 6. Ownership Examples

```bash
sudo chown username file.txt
sudo chgrp groupname file.txt
```

## 7. Practical Commands

```bash
mkdir permission-lab
cd permission-lab
touch notes.txt
ls -l
chmod 644 notes.txt
chmod 600 notes.txt
stat notes.txt
umask
```

## 8. DevOps Importance

- Securing Linux servers.
- Managing file access.
- Protecting SSH private keys.
- Controlling application permissions.
- Maintaining server security.

## Conclusion
Linux permissions are essential for secure file management, system administration, and DevOps.
