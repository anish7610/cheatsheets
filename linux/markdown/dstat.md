# dstat Command Overview

`dstat` is a versatile command-line tool for monitoring system resources in real-time. It combines and replaces several older monitoring tools like `vmstat`, `iostat`, `netstat`, and others, providing comprehensive and customizable output.

## Common Options

| Option   | Description                                                                 |
|----------|-----------------------------------------------------------------------------|
| `-c`     | Show CPU statistics.                                                        |
| `-d`     | Show disk statistics.                                                       |
| `-n`     | Show network statistics.                                                    |
| `-m`     | Show memory usage.                                                          |
| `-p`     | Show process statistics like created and running processes.                 |
| `-r`     | Show I/O request statistics.                                                |
| `-t`     | Show time/date stamp.                                                       |
| `--full` | Show all statistics available.                                              |
| `--top-cpu` | Display the most CPU-intensive processes.                                |
| `--top-io`  | Display the most I/O-intensive processes.                                |

## Usage Examples

### Basic CPU and Memory Monitoring

To monitor CPU and memory usage simultaneously:

```bash
dstat -c -m
```

### Disk and Network Stats

To check disk and network statistics:

```bash
dstat -d -n
```

### Full Resource Monitoring

To get a comprehensive overview of most system resources:

```bash
dstat --full
```

### Monitor with a Timestamp

To include a timestamp with the output:

```bash
dstat -t -c -d
```

### Top CPU-Intensive Processes

To display the top CPU-intensive processes:

```bash
dstat --top-cpu
```

## Cheat Sheet

```markdown
# Basic Usage
dstat [options]

# Common Options
-c        # CPU statistics
-d        # Disk statistics
-n        # Network statistics
-m        # Memory usage
-p        # Process statistics
-t        # Time/date stamp

# Full Overview
dstat --full

# Monitor Top Processes
dstat --top-cpu
dstat --top-io
```

Use `dstat` to gain real-time insights into system performance, facilitating diagnostics and optimizations.
