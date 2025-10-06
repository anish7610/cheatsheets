# `lighttpd` Command Overview

`lighttpd` is a lightweight web server designed for speed, simplicity, and efficiency. It is ideal for serving static content and small web applications, often used in low-resource environments.

## Common Options

| Option        | Explanation                                                     |
|---------------|-----------------------------------------------------------------|
| `-f`          | Specifies the configuration file to use.                        |
| `-m`          | Sets the directory for dynamically loadable modules.            |
| `-D`          | Runs the server in the foreground (do not daemonize).           |
| `-t`          | Tests the configuration file for syntax errors.                 |
| `-v`          | Displays version information.                                   |
| `-p`          | Prints the parsed configuration file to standard output.        |

## Usage Examples

### Start Lighttpd with a Specific Configuration File

```bash
lighttpd -f /etc/lighttpd/lighttpd.conf
```

### Run in Foreground for Debugging

```bash
lighttpd -D -f /etc/lighttpd/lighttpd.conf
```

### Test Configuration for Syntax Errors

```bash
lighttpd -t -f /etc/lighttpd/lighttpd.conf
```

### Display Version Information

```bash
lighttpd -v
```

## Cheat Sheet

```plaintext
# Start server with a config file
lighttpd -f /path/to/config

# Run server in foreground
lighttpd -D -f /path/to/config

# Test config syntax
lighttpd -t -f /path/to/config

# Show version
lighttpd -v
```
