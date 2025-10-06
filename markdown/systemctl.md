# `systemctl` Command Overview

`systemctl` is a command-line utility used to inspect and control the `systemd` system and service manager. It is commonly used to start, stop, restart, enable, and disable services on a Linux system.

## Common Options

| Option        | Description                                       |
|---------------|---------------------------------------------------|
| `start`       | Starts a specified service immediately.           |
| `stop`        | Stops a specified running service immediately.    |
| `restart`     | Restarts a specified service.                     |
| `status`      | Shows the current status of a specified service.  |
| `enable`      | Enables a service to start at boot.               |
| `disable`     | Disables a service from starting at boot.         |
| `reload`      | Reloads the configuration of a specified service. |
| `list-units`  | Lists all loaded units.                           |
| `is-active`   | Checks if a specified service is active.          |

## Usage Examples

### Starting a Service
```bash
sudo systemctl start nginx.service
```

### Stopping a Service
```bash
sudo systemctl stop nginx.service
```

### Restarting a Service
```bash
sudo systemctl restart nginx.service
```

### Checking the Status of a Service
```bash
systemctl status nginx.service
```

### Enabling a Service to Start at Boot
```bash
sudo systemctl enable nginx.service
```

### Disabling a Service from Starting at Boot
```bash
sudo systemctl disable nginx.service
```

### Listing All Loaded Units
```bash
systemctl list-units
```

### Checking if a Service is Active
```bash
systemctl is-active nginx.service
```

## Cheat Sheet

```plaintext
Start a service:    sudo systemctl start [service]
Stop a service:     sudo systemctl stop [service]
Restart a service:  sudo systemctl restart [service]
Check status:       systemctl status [service]
Enable at boot:     sudo systemctl enable [service]
Disable at boot:    sudo systemctl disable [service]
List units:         systemctl list-units
Is active?          systemctl is-active [service]
```
