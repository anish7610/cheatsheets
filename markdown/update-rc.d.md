# `update-rc.d` Command

`update-rc.d` is a command-line utility in Linux used to manage the runlevel symlinks for service scripts in `/etc/init.d/`. It helps configure which services start during the boot process and at different runlevels.

## Common Options

| Option          | Explanation                                                      |
|-----------------|------------------------------------------------------------------|
| `defaults`      | Add symlinks for the script with default Debian runlevel settings. |
| `remove`        | Remove all symlinks for the script.                              |
| `disable`       | Disable a service by removing symlinks in `/etc/rc?.d/`.         |
| `enable`        | Enable a service by adding symlinks in `/etc/rc?.d/`.            |
| `-n`            | Dry run; show what would be done without making changes.         |
| `-f`            | Force; used with `remove` to forcefully remove even if active.   |

## Usage Examples

### Default Installation
```bash
sudo update-rc.d apache2 defaults
```
This command adds Apache2 to startup with default runlevel settings.

### Remove a Service
```bash
sudo update-rc.d apache2 remove
```
This command removes all startup symlinks for Apache2.

### Disable a Service
```bash
sudo update-rc.d apache2 disable
```
This disables Apache2 from automatically starting at boot.

### Enable a Disabled Service
```bash
sudo update-rc.d apache2 enable
```
This enables Apache2 to start automatically at boot again.

## Cheat Sheet

```sh
# Add a service with default settings
sudo update-rc.d [service] defaults

# Remove a service
sudo update-rc.d [service] remove

# Disable a service
sudo update-rc.d [service] disable

# Enable a service
sudo update-rc.d [service] enable
```

Use `update-rc.d` to manage service start-up configurations efficiently on Debian-based systems.
