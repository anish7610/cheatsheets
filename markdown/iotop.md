## `iotop` Command Overview

`iotop` is a Linux utility that displays real-time disk I/O usage by processes. It's useful for monitoring and diagnosing disk performance issues.

### Common Options

| Option      | Description                                                                 |
|-------------|-----------------------------------------------------------------------------|
| `-o`        | Show only processes or threads actually doing I/O.                          |
| `-b`        | Run in batch mode (useful for logging).                                     |
| `-n NUM`    | Set the number of iterations before `iotop` exits (works with `-b`).        |
| `-d SEC`    | Set the delay between updates in seconds.                                   |
| `-p PID`    | Only show I/O activity for specific process ID(s).                          |
| `-u USER`   | Only show I/O activity for specific user(s).                                |
| `-k`        | Display sizes in kilobytes.                                                 |
| `-t`        | Add a timestamp to each line (useful for batch mode).                       |

### Usage Examples

#### Show Active I/O Processes

Display only processes performing I/O:

```bash
iotop -o
```

#### Monitor I/O in Batch Mode

Log I/O usage every 5 seconds for 3 iterations:

```bash
iotop -b -n 3 -d 5 > iotop.log
```

#### Monitor I/O for a Specific User

Display I/O activity of processes belonging to "username":

```bash
iotop -u username
```

#### Watch a Specific Process

Monitor a single process with a process ID of 1234:

```bash
iotop -p 1234
```

### Cheat Sheet

```bash
# Show active I/O processes
iotop -o

# Batch mode with delay of 3 seconds
iotop -b -n 5 -d 3

# Monitor specific user
iotop -u username

# Monitor specific process
iotop -p PID
```

This guide provides a quick reference to using `iotop` effectively for monitoring disk I/O activity in a Linux environment.
