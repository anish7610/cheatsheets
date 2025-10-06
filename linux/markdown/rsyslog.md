# `rsyslog` Command Cheat Sheet

## Description

`rsyslog` is a high-performance logging utility for Linux and Unix systems. It is used to forward log messages in an IP network, allowing for complex log filtering, classification, and analysis.

## Common Options

| Option                     | Description                                               |
|----------------------------|-----------------------------------------------------------|
| `-f /path/to/file`         | Specify the configuration file to use.                    |
| `-n`                       | Start in foreground mode, useful for debugging.           |
| `-c compatibility_version` | Set the backward-compatibility version.                   |
| `-N level`                 | Enable configuration checking only, useful for testing configurations. Levels: `1`, `2`, `3`. |
| `-d`                       | Enable debugging mode for diagnosing issues.              |

## Usage Examples

### Start rsyslog with a Specific Configuration File

```bash
rsyslogd -f /etc/rsyslog.d/my_custom_config.conf
```

### Test Configuration for Syntax Errors

```bash
rsyslogd -N 1
```

### Run rsyslog in Foreground for Debugging

```bash
rsyslogd -n
```

### Start rsyslog with Debugging Enabled

```bash
rsyslogd -d
```

## Quick Reference

```bash
# Start with specific config
rsyslogd -f /path/to/config

# Check configuration syntax
rsyslogd -N 1

# Run in foreground
rsyslogd -n

# Enable debug mode
rsyslogd -d
```

Adjust configurations and usage according to your system requirements and preferences.
