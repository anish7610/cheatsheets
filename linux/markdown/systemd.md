# `systemd` Command Overview

`systemd` is a system and service manager for Linux, responsible for bootstrapping the user space and managing system processes after booting. It is designed to start services in parallel, reduce shell overhead, and improve system performance.

## Common Options

| Option          | Description                                     |
|-----------------|-------------------------------------------------|
| `--version`     | Shows the version of `systemd`.                 |
| `--system`      | Connects to the system manager.                 |
| `--user`        | Connects to the user service manager instance.  |
| `--unit`        | Operates on the specified unit.                 |
| `--property`    | Indicates a property state to modify or view.   |
| `--test`        | Tests basic `systemd` functionality.            |

## Usage Examples

### Check systemd Version
```bash
systemd --version
```

### Start a Service
Start the `httpd` service:
```bash
systemctl start httpd
```

### Stop a Service
Stop the `nginx` service:
```bash
systemctl stop nginx
```

### Enable a Service at Boot
Enable the `mariadb` service to start at boot:
```bash
systemctl enable mariadb
```

### Disable a Service
Disable the `bluetooth` service from starting at boot:
```bash
systemctl disable bluetooth
```

### Check Service Status
Check the status of the `ssh` service:
```bash
systemctl status ssh
```

## Cheat Sheet

```plaintext
# Show version
systemd --version

# Start a service
systemctl start [service]

# Stop a service
systemctl stop [service]

# Enable service to start at boot
systemctl enable [service]

# Disable service from starting at boot
systemctl disable [service]

# Check service status
systemctl status [service]
```

Replace `[service]` with the name of the relevant service you wish to manage.
