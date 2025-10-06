## `dnf` Command Overview

`dnf` (Dandified YUM) is a package manager for RPM-based Linux distributions that installs, updates, and removes packages while handling dependencies automatically.

### Common `dnf` Options

| Option             | Description                                               |
|--------------------|-----------------------------------------------------------|
| `install`          | Installs one or more packages.                            |
| `remove`           | Removes one or more packages.                             |
| `update`           | Updates all packages or specified packages.               |
| `upgrade`          | Simultaneously upgrades and removes obsolete packages.    |
| `check-update`     | Checks for available updates.                             |
| `list`             | Lists software packages.                                  |
| `search`           | Searches for packages containing a specified string.      |
| `info`             | Displays detailed information about a package.            |
| `clean`            | Cleans up cached files.                                   |
| `autoremove`       | Removes unused dependencies.                              |
| `downgrade`        | Downgrades a package to an earlier version.               |
| `history`          | Shows transaction history.                                |

### Usage Examples

#### Installing a Package
```bash
sudo dnf install nginx
```

#### Removing a Package
```bash
sudo dnf remove nginx
```

#### Updating All Packages
```bash
sudo dnf update
```

#### Upgrading the Entire System
```bash
sudo dnf upgrade
```

#### Checking for Available Updates
```bash
dnf check-update
```

#### Searching for a Package
```bash
dnf search editor
```

#### Displaying Package Information
```bash
dnf info nginx
```

#### Cleaning Cached Files
```bash
sudo dnf clean all
```

#### Removing Unused Dependencies
```bash
sudo dnf autoremove
```

### Cheat Sheet

```plaintext
# Install a package
sudo dnf install <package>

# Remove a package
sudo dnf remove <package>

# Update packages
sudo dnf update

# Upgrade system
sudo dnf upgrade

# Check for updates
dnf check-update

# List packages
dnf list available|installed|all

# Search for a package
dnf search <string>

# Show package info
dnf info <package>

# Clean cache
sudo dnf clean all

# Remove unused dependencies
sudo dnf autoremove
```
