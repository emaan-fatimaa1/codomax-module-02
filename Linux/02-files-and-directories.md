# Linux: Files and Directories

## 1. Introduction
Linux uses a hierarchical file system to organize files and directories. Everything starts from the root directory (`/`).

## 2. Important Commands

| Command | Purpose |
|---|---|
| `pwd` | Displays the current working directory. |
| `ls` | Lists files and directories. |
| `ls -l` | Displays detailed file information. |
| `ls -a` | Shows hidden files and directories. |
| `cd` | Changes the current directory. |
| `cd ..` | Moves to the parent directory. |
| `cd ~` | Moves to the home directory. |
| `mkdir` | Creates a new directory. |
| `touch` | Creates an empty file. |
| `cp` | Copies files and directories. |
| `mv` | Moves or renames files and directories. |
| `rm` | Deletes files. |
| `rmdir` | Removes an empty directory. |
| `rm -r` | Removes a directory and its contents. |
| `cat` | Displays file contents. |

## 3. Absolute and Relative Paths

- **Absolute Path:** The complete path starting from the root directory (`/`).
- **Relative Path:** The path based on the current working directory.

## 4. Important Concepts

- `/` – Root directory.
- `~` – Current user's home directory.
- `.` – Current directory.
- `..` – Parent directory.
- Hidden files – Files whose names start with a dot (`.`).

## 5. Practical Commands

```bash
pwd
ls -la
mkdir practice
cd practice
touch file1.txt
mkdir projects
cp file1.txt projects/
mv file1.txt notes.txt
cat notes.txt
cd ..
rmdir practice/projects
rm practice/notes.txt
rmdir practice
```

## 6. Why Is This Important in DevOps?

Linux file and directory management is essential for:

- Managing application files on Linux servers.
- Organizing project directories.
- Working with configuration files.
- Managing logs and system files.
- Deploying and maintaining applications.

## Conclusion

Understanding Linux file and directory management is a fundamental skill for system administration, cloud computing, and DevOps.
