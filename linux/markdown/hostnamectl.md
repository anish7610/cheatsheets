# `hostnamectl` Command Overview

`hostnamectl` is a command-line utility in Linux used to query and change the system hostname, as well as to display system information.

## Common Options

| Option           | Description                                                      |
|------------------|------------------------------------------------------------------|
| `status`         | Display the current system hostname and other system information.|
| `set-hostname`   | Set a new static hostname for the system.                        |
| `set-icon-name`  | Set an icon name for the machine.                                |
| `set-chassis`    | Define the chassis type (e.g., `desktop`, `laptop`).             |
| `set-deployment` | Specify the current deployment environment (e.g., `production`). |

## Usage Examples

### Display Current Hostname and System Info
```bash
hostnamectl status
```

### Change the System Hostname
```bash
sudo hostnamectl set-hostname new-hostname
```

### Set the Icon Name of the Machine
```bash
sudo hostnamectl set-icon-name computer
```

### Define the Chassis Type
```bash
sudo hostnamectl set-chassis laptop
```

### Set the Deployment Environment
```bash
sudo hostnamectl set-deployment development
```

## Cheat Sheet

```plaintext
# Get current system info
hostnamectl status

# Change hostname
sudo hostnamectl set-hostname <new-hostname>

# Set icon name
sudo hostnamectl set-icon-name <icon>

# Set chassis type
sudo hostnamectl set-chassis <type>

# Set deployment environment
sudo hostnamectl set-deployment <environment>
```
