# `logrotate` Command Overview

The `logrotate` command in Linux is used to manage the automatic rotation and compression of log files. It helps in preventing log files from consuming excessive disk space by archiving, compressing, and removing old log entries.

## Common Options

| Option      | Description                                                                 |
|-------------|-----------------------------------------------------------------------------|
| `-d`        | Enables debug mode, showing what `logrotate` would do, without performing actions. |
| `-f`        | Forces rotation, even if it is not necessary according to the log file's age or size. |
| `-s <file>` | Uses the specified state file (which tracks when logs were last rotated).   |
| `-v`        | Increases verbosity (provides detailed logs of actions taken).              |
| `-m <cmd>`  | Specifies a command to mail the log files to after rotation.                |

## Usage Examples

### Basic Rotation
To rotate logs using a configuration file:
```bash
logrotate /etc/logrotate.conf
```

### Force Rotation
To forcefully rotate logs regardless of other conditions:
```bash
logrotate -f /etc/logrotate.conf
```

### Debug Mode
To see what actions `logrotate` would perform without executing them:
```bash
logrotate -d /etc/logrotate.conf
```

### Using a Custom State File
To use a specific state file:
```bash
logrotate -s /var/lib/logrotate.state /etc/logrotate.conf
```

## Cheat Sheet

```markdown
# Check configuration
logrotate -d /etc/logrotate.conf

# Force log rotation
logrotate -f /etc/logrotate.conf

# Use a specific state file
logrotate -s /var/lib/logrotate.state /etc/logrotate.conf

# Increase verbosity
logrotate -v /etc/logrotate.conf
```

Keep your logs manageable by customizing your rotation settings in `/etc/logrotate.conf` or supplementary configuration files in `/etc/logrotate.d/`.
