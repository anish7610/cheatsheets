# `logger` Command in Linux

The `logger` command is used to make entries in the system log. It allows you to log messages from the command line, scripts, or applications to the system logger, typically `syslog`.

## Common Options

| Option    | Description                                                      |
|-----------|------------------------------------------------------------------|
| `-p`      | Specify the priority (e.g., `user.notice`).                      |
| `-t`      | Add a tag to identify the message source.                        |
| `-f`      | Log the contents of a specified file.                            |
| `-i`      | Log the process ID with each message.                            |
| `--stderr`| Output the message to standard error as well.                    |
| `-n`      | Specify a remote logging host.                                   |

## Usage Examples

### Log a Simple Message
```bash
logger "System backups completed successfully."
```

### Log with Priority
```bash
logger -p user.warning "Low disk space on server."
```

### Add a Tag
```bash
logger -t backup-script "Backup started at $(date)"
```

### Log the Contents of a File
```bash
logger -f /path/to/logfile
```

### Include Process ID
```bash
logger -i "The service has started."
```

### Log to a Remote Host
```bash
logger -n 192.168.1.100 "Remote logging test message."
```

## Cheat Sheet

```plaintext
# Log a simple message
logger "message"

# Specify priority
logger -p [facility.priority] "message"

# Add a tag
logger -t [tagname] "message"

# Log file contents
logger -f [file]

# Include PID
logger -i "message"

# Log to remote host
logger -n [hostname] "message"
```
