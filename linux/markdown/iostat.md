## `iostat` Command Overview

The `iostat` command in Linux is used to monitor system I/O device loading. It provides statistics for CPU and I/O device utilization, which can help identify bottlenecks in the system's input/output performance.

## Common Options

| Option     | Description                                                |
|------------|------------------------------------------------------------|
| `-c`       | Displays only the CPU statistics.                          |
| `-d`       | Shows only device utilization reports.                     |
| `-x`       | Provides extended statistics for devices.                  |
| `-k`       | Displays statistics in kilobytes per second.               |
| `-m`       | Displays statistics in megabytes per second.               |
| `-t`       | Includes a timestamp with each report.                     |
| `-h`       | Produces a human-readable output.                          |

## Usage Examples

### Basic Device Utilization
```bash
iostat -d
```
This command shows the current device utilization report, providing basic I/O stats.

### CPU and Device Utilization
```bash
iostat -c -d
```
Displays both CPU statistics and device utilization information.

### Extended Device Statistics
```bash
iostat -x
```
Offers detailed I/O statistics for each device, useful for diagnosing performance issues.

### Timestamped Reports
```bash
iostat -t 2 5
```
Generates a report every 2 seconds, repeating 5 times, each with a timestamp.

### Human-Readable Output
```bash
iostat -h
```
Presents the statistics in a more readable format with appropriate unit labels.

## Cheat Sheet

```plaintext
iostat -d        # Device report
iostat -c        # CPU report
iostat -x        # Extended device stats
iostat -t <sec>  # Timestamped output
```
