# Apache2 Command Overview

The `apache2` command is used to start the Apache HTTP server, manage its configuration, and control its operation. It is a key tool for administering web servers running on Linux systems.

## Common Options

| Option      | Description                                              |
|-------------|----------------------------------------------------------|
| `-k start`  | Starts the Apache server if not already running.         |
| `-k stop`   | Stops the Apache server if it is currently running.      |
| `-k restart`| Restarts the Apache server.                              |
| `-k graceful`| Gracefully restarts the Apache server. Avoids dropping connections. |
| `-k graceful-stop` | Gracefully stops the server, finishing existing requests. |
| `-v`        | Displays the version of Apache being used.               |
| `-V`        | Displays build parameters for Apache.                    |
| `-t`        | Checks the syntax of the configuration files.            |
| `-S`        | Shows a summary of the virtual hosts configurations.     |

## Usage Examples

### Start the Apache Server
```bash
sudo apache2 -k start
```

### Stop the Apache Server
```bash
sudo apache2 -k stop
```

### Restart the Apache Server
```bash
sudo apache2 -k restart
```

### Check Configuration Syntax
```bash
sudo apache2 -t
```

### Show Virtual Hosts Summary
```bash
sudo apache2 -S
```

## Cheat Sheet

```plaintext
Start:    sudo apache2 -k start
Stop:     sudo apache2 -k stop
Restart:  sudo apache2 -k restart
Config Check: sudo apache2 -t
VHosts:   sudo apache2 -S
Version:  apache2 -v
```
