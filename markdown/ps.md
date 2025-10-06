# `ps` Command Overview

The `ps` command in Linux is used to display information about active processes. It provides a snapshot of current processes, allowing users to view process IDs (PIDs), CPU usage, execution time, and more.

## Common Options

| Option  | Description                                                |
|---------|------------------------------------------------------------|
| `-e`    | Show information about all processes.                      |
| `-f`    | Display full-format listing.                               |
| `-u`    | Specify a user whose processes are to be viewed.           |
| `-x`    | Show processes without a controlling terminal.             |
| `-aux`  | Show all processes for all users, including those not attached to a terminal. |
| `-p`    | Select by PID. Display information for the specified PIDs. |
| `-o`    | Format the output using a user-defined format.             |
| `--sort`| Sort output by a specific field(s).                        |

## Usage Examples

### View All Processes

```bash
ps -e
```

### Full-Format Listing

```bash
ps -ef
```

### Processes by a Specific User

```bash
ps -u username
```

### All Processes Without Terminal

```bash
ps -x
```

### All Processes with Custom Format

```bash
ps -eo pid,comm,pmem
```

### View Specific Process by PID

```bash
ps -p 1234
```

### Sort Processes by Memory Usage

```bash
ps aux --sort=-%mem
```

## Cheat Sheet

```plaintext
ps -e          # Show all processes
ps -ef         # Full-format listing
ps -u user     # Processes for specific user
ps -x          # Processes without terminal
ps aux         # All processes for all users
ps -p 1234     # Process with PID 1234
ps -eo pid,cmd # Custom format output
ps aux --sort=-%mem # Sort by memory usage
```
