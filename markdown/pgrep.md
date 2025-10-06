# `pgrep` Command Overview

`pgrep` is a Linux command-line utility used to search for processes currently running on the system based on name and other attributes. It returns the process IDs (PIDs) of matching processes, allowing users to quickly identify and manage processes.

## Common Options

| Option   | Description                                                      |
|----------|------------------------------------------------------------------|
| `-f`     | Match against the full command line (including arguments).      |
| `-l`     | List PIDs and the process names.                                |
| `-a`     | List PIDs with full command line arguments.                     |
| `-v`     | Invert the match, showing processes that do not match the criteria. |
| `-u`     | Match only processes whose effective user ID is listed.         |
| `-x`     | Match the exact process name.                                   |
| `-n`     | Show only the most recently started matching process.           |
| `-o`     | Show only the oldest (first started) matching process.          |

## Usage Examples

- **Find PIDs of all `sshd` processes:**
  ```bash
  pgrep sshd
  ```

- **Find PIDs of processes with a specific user:**
  ```bash
  pgrep -u username
  ```

- **Find PIDs with full command line arguments:**
  ```bash
  pgrep -a sshd
  ```

- **Find the most recently started process named `nginx`:**
  ```bash
  pgrep -n nginx
  ```

- **Find processes except the ones named `bash`:**
  ```bash
  pgrep -v bash
  ```

## Cheat Sheet

```bash
pgrep [OPTIONS] <pattern>

# Find process by name:
pgrep <name>

# Full command line match:
pgrep -f <pattern>

# PIDs with process name:
pgrep -l <name>

# PIDs with full command line:
pgrep -a <name>
```
