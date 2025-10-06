# `logcheck` Command Overview

`logcheck` is a tool for monitoring log files and alerting the system administrator to unusual activities or errors by filtering out normal log entries based on predefined rules.

## Common Options

| Option           | Description                                                   |
|------------------|---------------------------------------------------------------|
| `-d`, `--daemon` | Run in daemon mode, continuously checking logs.               |
| `-o`, `--open`   | When in daemon mode, keep the log file open.                  |
| `-q`, `--quiet`  | Suppress output when no messages are found.                   |
| `-r`, `--reload` | Reload rules and signals for log re-evaluation.               |
| `-s`, `--syslog` | Use syslog for errors and status notifications.               |
| `-t`, `--test`   | Test mode to check configuration and rule syntax.             |

## Usage Examples

### Basic Check
```bash
logcheck
```
Run `logcheck` manually to analyze logs and send a report.

### Daemon Mode
```bash
logcheck --daemon
```
Operate `logcheck` continuously in the background.

### Reload Rules
```bash
logcheck --reload
```
Reload rules without restarting the `logcheck` service.

### Suppress Output
```bash
logcheck --quiet
```
Run `logcheck` but only output messages when there are alerts.

## Cheat Sheet

```plaintext
# Run logcheck in daemon mode
logcheck --daemon

# Reload rules for logcheck
logcheck --reload

# Test logcheck configuration
logcheck --test

# Quiet mode: No output when there are no alerts
logcheck --quiet
```

Use these commands responsibly to maintain awareness of unusual system behavior and potentially catch security issues early on.
