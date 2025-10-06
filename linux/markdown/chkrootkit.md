# `chkrootkit` Command in Linux

`chkrootkit` is a tool used to check for signs of rootkit infections on Unix-based systems. Rootkits are malicious software designed to gain unauthorized root access.

## Common Options

| Option       | Explanation                                          |
|--------------|------------------------------------------------------|
| `-q`         | Quiet mode; only show suspected results.             |
| `-x`         | Expert mode; show a detailed process of checks.      |
| `-r <dir>`   | Specify an alternative root directory to check.      |
| `-l`         | List all tests available in `chkrootkit`.            |
| `-h`         | Display help information.                            |
| `-d`         | Debug mode; provide more detailed information.       |
| `-p <dir>`   | Path for the external command binaries.              |

## Usage Examples

### Basic Check
To perform a basic rootkit scan on the system:
```bash
sudo chkrootkit
```

### Quiet Mode
To run `chkrootkit` in quiet mode, showing only suspected infections:
```bash
sudo chkrootkit -q
```

### Check Specific Directory
To check a non-default root directory (e.g., a mounted backup):
```bash
sudo chkrootkit -r /mnt/backup
```

### List All Tests
To list all the checks that `chkrootkit` performs:
```bash
chkrootkit -l
```

### Expert Mode
For a more detailed output of the checks:
```bash
sudo chkrootkit -x
```

## Cheat Sheet

```plaintext
sudo chkrootkit          # Basic check for rootkits
sudo chkrootkit -q       # Quiet mode for suspected rootkits
sudo chkrootkit -r /dir  # Check specific directory
chkrootkit -l            # List all tests
sudo chkrootkit -x       # Run in expert mode
```
