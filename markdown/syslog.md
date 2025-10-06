# syslog Command in Linux

`syslog` is not a standalone command but a protocol used by various logging utilities like `rsyslog`, `syslog-ng`, and `systemd-journald` to manage logs. These utilities provide mechanisms to collect, store, and process log messages from different sources.

## Common `syslog` Options

When working with utilities that implement syslog, here are some options, assuming usage with `logger` (a command-line tool for sending logs to syslog):

| Option      | Explanation                            |
|-------------|----------------------------------------|
| `-p`        | Specify the priority (e.g., auth.info) |
| `-t`        | Include a tag to identify the log      |
| `-f`        | Log the contents of a specified file   |
| `-i`        | Include process ID in the log message  |
| `-s`        | Log message to stderr as well          |

## Usage Examples

### Sending a Simple Log Message
```bash
logger "System maintenance completed"
```

### Specifying a Priority Level
```bash
logger -p local0.notice "Disk space updated"
```

### Tagging a Log Message
```bash
logger -t BACKUP "Backup operation started"
```

### Logging the Contents of a File
```bash
logger -f /var/log/example.log
```

### Including a Process ID in the Message
```bash
logger -i "Service restarted"
```

## Cheat Sheet

```bash
# Log a simple message
logger "Your message here"

# Log with specific priority
logger -p service.info "Service started"

# Log with a custom tag
logger -t MYTAG "Tagged message"

# Log contents of a file
logger -f /path/to/file

# Log message including process ID
logger -i "Process info"
```
