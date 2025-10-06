# Bacula Command Overview

`Bacula` is a set of programs to manage backup, recovery, and verification of data across a network of computers. It is efficient for large-scale data management tasks.

## Common Options

| Option            | Description                                         |
|-------------------|-----------------------------------------------------|
| `-c <config-file>`| Specify configuration file to use.                  |
| `-d <debug-level>`| Set debug level for verbose output.                 |
| `-t`              | Test configuration files without executing.         |
| `-f`              | Run in the foreground, not as a daemon.             |
| `-s`              | Simulate actions without actually performing them.  |

## Usage Examples

### Example 1: Running Bacula with a Specific Configuration
```bash
bacula-dir -c /etc/bacula/bacula-dir.conf
```

### Example 2: Testing Configuration Files for Errors
```bash
bacula-dir -t -c /etc/bacula/bacula-dir.conf
```

### Example 3: Running Bacula in Debug Mode
```bash
bacula-dir -d 100 -c /etc/bacula/bacula-dir.conf
```

## Cheat Sheet

```markdown
# Start Bacula with a config
bacula-dir -c <config-file>

# Test config without executing
bacula-dir -t -c <config-file>

# Run with verbose debug output
bacula-dir -d <level> -c <config-file>

# Simulate the actions
bacula-dir -s -c <config-file>
```
