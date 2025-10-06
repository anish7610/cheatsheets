# Snap Command Overview

`snap` is a package management system for installing and managing applications in a Linux distribution. It operates with "snaps", which are application packages that work across multiple Linux distros.

---

## Common Options

| Option               | Explanation                                           |
|----------------------|-------------------------------------------------------|
| `install <package>`  | Installs the specified snap package.                  |
| `remove <package>`   | Removes the specified snap package.                   |
| `refresh`            | Updates installed snap packages to the latest version.|
| `list`               | Lists all installed snap packages.                    |
| `find <package>`     | Searches for a snap package in the store.             |
| `info <package>`     | Displays detailed information about a snap package.   |

---

## Usage Examples

### Installing a Snap Package

```bash
snap install vlc
```

### Removing a Snap Package

```bash
snap remove vlc
```

### Updating All Snap Packages

```bash
snap refresh
```

### Listing Installed Snaps

```bash
snap list
```

### Searching for a Snap Package

```bash
snap find spotify
```

### Getting Information About a Snap Package

```bash
snap info vlc
```

---

## Cheat Sheet

```plaintext
snap install <package>    # Install a package
snap remove <package>     # Remove a package
snap refresh              # Update packages
snap list                 # List all installed packages
snap find <package>       # Search for packages
snap info <package>       # Get package details
```
