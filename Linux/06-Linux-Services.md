# Linux Services

### 1. What Are Services?
Services are background programs that perform specific tasks without requiring direct user interaction.

**Examples:**
- SSH – Allows remote access to a Linux server.
- Nginx – Hosts websites.
- Cron – Runs scheduled tasks.
- Docker – Manages containers.

### 2. systemd and systemctl
- **systemd:** The system and service manager in Linux.
- **systemctl:** A command-line tool used to manage services.

### 3. Managing Services

| Command | Purpose |
|---|---|
| `systemctl status nginx` | Check service status |
| `sudo systemctl start nginx` | Start a service |
| `sudo systemctl stop nginx` | Stop a service |
| `sudo systemctl restart nginx` | Restart a service |
| `sudo systemctl reload nginx` | Reload configuration |
| `sudo systemctl enable nginx` | Enable service at boot |
| `sudo systemctl disable nginx` | Disable service at boot |
| `sudo systemctl enable --now nginx` | Enable and start service |
| `systemctl is-active nginx` | Check if service is running |
| `systemctl is-enabled nginx` | Check if service starts at boot |

### 4. Listing Services

```bash
systemctl list-units --type=service
systemctl list-units --type=service --all
systemctl list-unit-files --type=service
```

### 5. Viewing Service Logs

Linux uses `journalctl` to view system and service logs.

```bash
journalctl -u nginx
journalctl -u nginx -n 20
journalctl -u nginx -f
```

- `-u`: Shows logs for a specific service.
- `-n 20`: Displays the last 20 log entries.
- `-f`: Follows logs in real time.

### 6. Service Unit Files

Systemd uses unit files to define how services should run.

Common locations:
- `/usr/lib/systemd/system/`
- `/etc/systemd/system/`

View a service's unit file:

```bash
systemctl cat nginx
```

After modifying a unit file, run:

```bash
sudo systemctl daemon-reload
```

This reloads systemd's configuration.

### 7. Mask and Unmask Services

```bash
sudo systemctl mask nginx
sudo systemctl unmask nginx
```

- `mask`: Prevents a service from being started.
- `unmask`: Removes this restriction.

### 8. Troubleshooting Services

A basic troubleshooting process:

1. Check service status.
2. Review service logs.
3. Check configuration.
4. Restart the service if required.
5. Verify that it is running.

### 9. Importance in Cloud and DevOps

Service management is important because:

- Cloud servers use services to run applications.
- DevOps engineers manage services such as Nginx, Docker and SSH.
- Logs help identify and troubleshoot errors.
- Services can be configured to start automatically when a server boots.

**Conclusion:** Linux service management helps administrators start, stop, monitor, configure and troubleshoot background services on Linux servers.
