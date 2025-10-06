# Choco Command Overview

`choco` is a command-line interface (CLI) for Chocolatey, a package manager for Windows. It helps automate the installation and management of software on Windows systems.

## Common Options

| Option                  | Explanation                                           |
|-------------------------|-------------------------------------------------------|
| `install <package>`     | Installs a package.                                   |
| `upgrade <package>`     | Upgrades an existing package to the latest version.   |
| `uninstall <package>`   | Uninstalls a package.                                 |
| `list`                  | Lists installed packages.                             |
| `search <term>`         | Searches for a package matching the given term.       |
| `info <package>`        | Shows information about a specific package.           |
| `version`               | Displays the version of Chocolatey.                   |

## Usage Examples

### Installing a Package

```bash
choco install git
```

### Upgrading All Packages

```bash
choco upgrade all
```

### Uninstalling a Package

```bash
choco uninstall googlechrome
```

### Listing Installed Packages

```bash
choco list --localonly
```

### Searching for a Package

```bash
choco search vscode
```

### Getting Package Information

```bash
choco info nodejs
```

## Cheat Sheet

```
# Install a package
choco install <package>

# Upgrade a package
choco upgrade <package>

# Upgrade all packages
choco upgrade all

# Uninstall a package
choco uninstall <package>

# List installed packages
choco list --localonly

# Search for a package
choco search <term>

# Get information on a package
choco info <package>
```
