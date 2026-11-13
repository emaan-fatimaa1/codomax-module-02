# Linux Process Management

### 1. Finding Processes
| Command | Purpose |
|---|---|
| `pgrep nginx` | Find process by name |
| `pidof nginx` | Find process PID |
| `pstree -p` | Show process hierarchy with PIDs |

### 2. Managing Processes
| Command | Purpose |
|---|---|
| `kill PID` | Gracefully terminate process |
| `kill -9 PID` | Forcefully terminate process |
| `pkill nginx` | Terminate by process name |
| `jobs` | Show background jobs |
| `bg` | Resume job in background |
| `fg` | Bring job to foreground |

### 3. Background Processes
- `command &` – Run command in background.
- `Ctrl + Z` – Suspend foreground process.
- `nohup command &` – Keep command running after terminal disconnection.

### 4. Process Priority
- Nice value range: **-20 to +19**.
- `-20` = Highest scheduling preference.
- `+19` = Lowest scheduling preference.

| Command | Purpose |
|---|---|
| `nice -n 10 command` | Set priority when starting |
| `renice -n 10 -p PID` | Change existing process priority |

### 5. Cloud & DevOps Use
- Monitor CPU and RAM.
- Identify problematic processes.
- Troubleshoot Linux servers.
- Manage background applications.
- Control process priorities.
