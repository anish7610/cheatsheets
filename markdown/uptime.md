# `uptime` Command in Linux

The `uptime` command provides information about how long the system has been running, the number of users currently logged in, and the system load averages for the past 1, 5, and 15 minutes.

## Common Options

| Option | Explanation                           |
|--------|---------------------------------------|
| None   | Displays the default uptime information. |
| `-p`   | Shows uptime in a human-readable format. |
| `-s`   | Displays the date and time since when the system has been up. |

## Usage Examples

### Display Basic Uptime Information
```bash
uptime
```

### Display Uptime in a Human-Readable Format
```bash
uptime -p
```

### Show the Date and Time Since the System Was Last Started
```bash
uptime -s
```

## Cheat Sheet

```bash
# Basic uptime
uptime

# Human-readable format
uptime -p

# System start time
uptime -s
```

This concise format provides essential information quickly and efficiently, suitable for everyday use.
