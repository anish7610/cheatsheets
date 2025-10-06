# `sar` Command in Linux

The `sar` (System Activity Reporter) command is used to collect, report, and save system activity information. It provides a historical look at system performance, allowing users to analyze various resource usage metrics.

## Common Options

| Option       | Description                                              |
|--------------|----------------------------------------------------------|
| `-u`         | Report CPU utilization.                                  |
| `-r`         | Report memory usage statistics.                          |
| `-b`         | Report I/O and transfer rate.                            |
| `-n`         | Report network statistics, follow with `DEV` for devices.|
| `-q`         | Report load average and queue sizes.                     |
| `-d`         | Report activity for each block device.                   |
| `-p`         | When used with disk options, reports statistics per device. |
| `-f`         | Specify file to read data from (default: `/var/log/sa/sadd`).|

## Usage Examples

### Check CPU Usage
To report CPU utilization every 5 seconds for 3 iterations:
```bash
sar -u 5 3
```

### Check Memory Usage
To view memory usage statistics:
```bash
sar -r 1 3
```

### Check Network Statistics
To report network statistics for all devices every 1 second for 5 times:
```bash
sar -n DEV 1 5
```

### Disk Usage Statistics
To report block device statistics:
```bash
sar -d 1 3
```

## Cheat Sheet

```plaintext
sar -u N M      # CPU usage, every N seconds, M times
sar -r N M      # Memory stats, every N seconds, M times
sar -n DEV N M  # Network stats, every N seconds, M times
sar -d N M      # Disk stats, every N seconds, M times
```

Replace `N` with your desired interval and `M` with the number of data points to collect.
