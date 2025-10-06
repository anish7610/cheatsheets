# `apt-get` Command Overview

`apt-get` is a command-line tool for handling packages on Debian-based systems. It is used to install, update, and remove software packages.

## Common Options

| Option           | Description                                              |
|------------------|----------------------------------------------------------|
| `update`         | Updates the list of available packages and their versions. |
| `upgrade`        | Installs the newest versions of all currently installed packages. |
| `install`        | Installs one or more packages.                           |
| `remove`         | Removes one or more packages.                            |
| `autoremove`     | Removes automatically installed packages no longer needed. |
| `purge`          | Removes packages and their configuration files.          |
| `clean`          | Clears out the local repository of retrieved package files. |
| `dist-upgrade`   | Performs a distribution upgrade, handling dependencies intelligently. |
| `check`          | Checks for broken dependencies.                          |

## Usage Examples

### Update Package List
```bash
sudo apt-get update
```

### Upgrade Installed Packages
```bash
sudo apt-get upgrade
```

### Install a Package
```bash
sudo apt-get install package_name
```

### Remove a Package
```bash
sudo apt-get remove package_name
```

### Remove a Package and Configuration Files
```bash
sudo apt-get purge package_name
```

### Clean Package Cache
```bash
sudo apt-get clean
```

### Perform a Distribution Upgrade
```bash
sudo apt-get dist-upgrade
```

### Auto-remove Unnecessary Packages
```bash
sudo apt-get autoremove
```

## Cheat Sheet

```plaintext
# Update package list
sudo apt-get update

# Upgrade all packages
sudo apt-get upgrade

# Install a package
sudo apt-get install [package_name]

# Remove a package
sudo apt-get remove [package_name]

# Remove a package and its configuration files
sudo apt-get purge [package_name]

# Clean package cache
sudo apt-get clean
```
