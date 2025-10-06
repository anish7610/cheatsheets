# `journalctl` Command

`journalctl` is a utility for querying and displaying messages from the systemd journal, which stores logs related to services, applications, and the system.

## Common Options

| Option          | Description                                              |
|-----------------|----------------------------------------------------------|
| `-b`            | Show logs from the current boot.                         |
| `-k`            | Display only kernel messages.                            |
| `-u <unit>`     | Show logs for a specific systemd service/unit.           |
| `-f`            | Follow new log entries as they are added.                |
| `-n <number>`   | Show the last `<number>` of log entries.                 |
| `--since`       | Show logs since a certain date or time.                  |
| `--until`       | Show logs until a certain date or time.                  |
| `-p <priority>` | Show logs matching the specified priority.               |
| `-o <format>`   | Change output format, e.g., `short`, `json`.             |

## Usage Examples

### View Logs from the Current Boot
```bash
journalctl -b
```

### Show Kernel Messages
```bash
journalctl -k
```

### Display Logs for a Specific Service
```bash
journalctl -u nginx.service
```

### Follow Logs in Real-Time
```bash
journalctl -f
```

### View the Last 100 Log Entries
```bash
journalctl -n 100
```

### Show Logs Since a Specific Date
```bash
journalctl --since "2023-01-01"
```

### Display Logs with High Priority
```bash
journalctl -p 0..3
```

## Cheat Sheet

```bash
# Logs from current boot
journalctl -b

# Logs for a service
journalctl -u <service>

# Follow logs
journalctl -f

# Last N entries
journalctl -n <number>

# Logs since date
journalctl --since "<date>"

# High priority logs
journalctl -p 0..3
```
