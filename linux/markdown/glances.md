# Glances Command in Linux

`glances` is a cross-platform system monitoring tool that provides a real-time overview of various system metrics such as CPU, memory, disk I/O, network usage, and more.

## Common Options

| Option    | Explanation                                          |
|-----------|------------------------------------------------------|
| `-h`      | Display help information.                            |
| `-t`      | Set refresh time in seconds (default is 1 second).   |
| `-s`      | Start Glances in server mode for remote monitoring.  |
| `-c`      | Connect to a Glances server running in server mode.  |
| `--export`| Export data to external storage (e.g., CSV, InfluxDB).|
| `-f`      | Standalone mode (no web server).                     |

## Usage Examples

### Launch Glances with Default Settings

```bash
glances
```

### Set Refresh Time to 5 Seconds

```bash
glances -t 5
```

### Start Glances in Server Mode

```bash
glances -s
```

### Connect to a Remote Glances Server

```bash
glances -c 192.168.1.100
```

### Export Data to CSV

```bash
glances --export csv
```

## Cheat Sheet

```bash
# Basic Usage
glances

# Refresh every 5 seconds
glances -t 5

# Server mode
glances -s

# Connect to a server
glances -c [IP_ADDRESS]

# Export to CSV
glances --export csv
```
