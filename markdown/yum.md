# `yum` Command in Linux

`yum` (Yellowdog Updater Modified) is a package manager for RPM-based Linux distributions. It is used to install, update, remove, and manage software packages.

## Common Options

| Option         | Description                                           |
|----------------|-------------------------------------------------------|
| `install`      | Installs a package                                    |
| `update`       | Updates all packages or specified package             |
| `remove`       | Removes a package                                     |
| `list`         | Lists available, installed, or both categories        |
| `info`         | Displays detailed information about a package         |
| `search`       | Searches for a package by name or keyword             |
| `clean`        | Cleans up cached files                                |
| `check-update` | Checks for available updates                          |
| `repolist`     | Displays the list of configured repositories          |

## Usage Examples

### Install a Package
```bash
yum install package-name
```

### Update All Packages
```bash
yum update
```

### Update a Specific Package
```bash
yum update package-name
```

### Remove a Package
```bash
yum remove package-name
```

### Search for a Package
```bash
yum search keyword
```

### List Installed Packages
```bash
yum list installed
```

### Get Information about a Package
```bash
yum info package-name
```

### Clean Cached Files
```bash
yum clean all
```

## Cheat Sheet

```plaintext
yum install package-name  # Install
yum update                # Update all
yum update package-name   # Update specific
yum remove package-name   # Remove
yum search keyword        # Search
yum list installed        # List installed
yum info package-name     # Info about package
yum clean all             # Clean cache
yum repolist              # List repositories
```
