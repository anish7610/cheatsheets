# `httpd` Command in Linux

`httpd` is a command used to start the Apache HTTP Server, which is a widely-used open source web server. This command is crucial for managing the Apache server, including starting, stopping, and configuring it.

## Common Options

| Option       | Description                                               |
|--------------|-----------------------------------------------------------|
| `-k start`   | Starts the Apache HTTP server.                            |
| `-k stop`    | Stops the Apache HTTP server.                             |
| `-k restart` | Restarts the Apache server (stops and then starts again). |
| `-k graceful`| Gracefully restarts the Apache server without dropping connections. |
| `-f`         | Specifies an alternate configuration file.                |
| `-v`         | Displays the version number and exits.                    |
| `-h`         | Displays a help message with available options.           |

## Usage Examples

### Start the Apache Server
```bash
httpd -k start
```

### Stop the Apache Server
```bash
httpd -k stop
```

### Restart the Apache Server
```bash
httpd -k restart
```

### Graceful Restart of the Server
```bash
httpd -k graceful
```

### Use an Alternate Configuration File
```bash
httpd -f /path/to/custom/httpd.conf
```

### Check the Version of Apache
```bash
httpd -v
```

## Cheat Sheet

```bash
# Start Apache
httpd -k start

# Stop Apache
httpd -k stop

# Restart Apache
httpd -k restart

# Graceful restart
httpd -k graceful

# Use custom config file
httpd -f /path/to/httpd.conf
```

This encapsulates the essentials for using the `httpd` command in everyday scenarios.
