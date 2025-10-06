# `vmstat` Command in Linux

## Description

`vmstat` (Virtual Memory Statistics) is a command-line utility that reports virtual memory statistics. It provides information about processes, memory, paging, block IO, traps, and CPU activity.

## Common Options

| Option       | Description                                                             |
|--------------|-------------------------------------------------------------------------|
| `-a`         | Displays active and inactive memory.                                     |
| `-s`         | Provides a summary of memory statistics.                                 |
| `-d`         | Displays disk statistics.                                                |
| `-p <device>`| Shows statistics for a specific block device.                            |
| `-t`         | Adds a timestamp to the reports.                                         |
| `-w`         | Provides a summary of system swapping statistics.                        |
| `-S <unit>`  | Sets the unit for display (e.g., k for kilobytes, m for megabytes).      |

## Usage Examples

### Basic Usage
Displays a snapshot of system performance:
```bash
vmstat
```

### Continuous Monitoring
Runs `vmstat` every 5 seconds, displaying 10 updates:
```bash
vmstat 5 10
```

### Viewing Disk Statistics
Lists disk statistics:
```bash
vmstat -d
```

### Viewing Memory Summary
Displays a summary of memory:
```bash
vmstat -s
```

### Active and Inactive Memory
Shows active and inactive memory:
```bash
vmstat -a
```

### Monitor Specific Device
Monitors statistics for a specific block device:
```bash
vmstat -p /dev/sda
```

### Adding a Timestamp
Provides a timestamp with each update:
```bash
vmstat -t 5 5
```

## Cheat Sheet

```plaintext
# Basic Snapshot
vmstat

# Continuous Monitoring (5s interval, 10 times)
vmstat 5 10

# Disk Stats
vmstat -d

# Memory Summary
vmstat -s

# Active & Inactive Memory
vmstat -a

# Specific Device Stats
vmstat -p /dev/sda

# Timestamped Output
vmstat -t 5 5
```
