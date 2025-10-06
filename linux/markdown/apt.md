# `apt` Command in Linux

`apt` is a command-line interface used to handle packages on Debian-based systems, such as Ubuntu. It simplifies package management tasks including installation, updates, and removal of software.

## Common Options

| Option         | Description                                                    |
|----------------|----------------------------------------------------------------|
| `update`       | Updates the package lists for upgrades and new package installations. |
| `upgrade`      | Installs the latest versions of all currently installed packages. |
| `install`      | Installs one or more packages.                                 |
| `remove`       | Removes one or more packages.                                  |
| `autoremove`   | Removes packages that were automatically installed to satisfy dependencies and are no longer needed. |
| `purge`        | Removes packages and their configuration files.                |
| `search`       | Searches the package list for a given term.                    |
| `show`         | Displays detailed information about a package.                 |
| `list`         | Lists available, installed, or upgradeable packages.           |
| `clean`        | Removes retrieved package files from the local cache.          |

## Usage Examples

### Update Package Lists
```bash
sudo apt update
```

### Upgrade Installed Packages
```bash
sudo apt upgrade
```

### Install a Package
```bash
sudo apt install htop
```

### Remove a Package
```bash
sudo apt remove htop
```

### Search for a Package
```bash
apt search vim
```

### Show Package Information
```bash
apt show curl
```

### Autoremove Unused Packages
```bash
sudo apt autoremove
```

## Cheat Sheet

```plaintext
sudo apt update               # Update package lists
sudo apt upgrade              # Upgrade all packages
sudo apt install <package>    # Install a package
sudo apt remove <package>     # Remove a package
sudo apt search <term>        # Search for a package
apt show <package>            # Show package info
sudo apt autoremove           # Remove unused packages
```
