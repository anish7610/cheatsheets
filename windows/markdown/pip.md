# `pip` Command Overview

`pip` is a package manager for Python that allows you to install, update, and manage Python packages from the Python Package Index (PyPI).

## Common Options

| Option               | Description                                                   |
|----------------------|---------------------------------------------------------------|
| `install`            | Install packages.                                             |
| `uninstall`          | Uninstall packages.                                           |
| `list`               | List installed packages.                                      |
| `show`               | Display information about installed packages.                 |
| `freeze`             | Output installed packages in requirements format.             |
| `--upgrade`          | Upgrade packages to the newest available version.             |
| `-r <file>`          | Install all packages listed in `<file>`.                      |
| `search`             | Search PyPI for packages.                                     |
| `check`              | Verify installed packages have compatible dependencies.       |

## Usage Examples

### Installing a Package

```bash
pip install requests
```

### Uninstalling a Package

```bash
pip uninstall requests
```

### Listing Installed Packages

```bash
pip list
```

### Displaying Package Details

```bash
pip show requests
```

### Freezing Installed Packages

```bash
pip freeze > requirements.txt
```

### Installing from a Requirements File

```bash
pip install -r requirements.txt
```

### Upgrading a Package

```bash
pip install --upgrade requests
```

### Searching for a Package

```bash
pip search requests
```

### Checking Package Compatibility

```bash
pip check
```

## Quick Reference Cheat Sheet

```plaintext
pip install <package>      # Install a package
pip uninstall <package>    # Remove a package
pip list                   # List all installed packages
pip show <package>         # Show detailed info
pip freeze                 # Output packages in requirements format
pip install -r <file>      # Install from requirements file
pip install --upgrade <package>  # Upgrade a package
pip search <package>       # Search for packages in PyPI
pip check                  # Check dependency compatibility
```
