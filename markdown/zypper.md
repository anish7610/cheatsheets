# Zypper Command

`zypper` is the command-line interface for package management in SUSE-based Linux distributions. It is used for installing, updating, and managing software packages.

## Common Options

| Option          | Description                                                                 |
|-----------------|-----------------------------------------------------------------------------|
| `install`       | Installs specified packages.                                                |
| `remove`        | Removes specified packages.                                                 |
| `update`        | Updates installed packages to the latest versions.                          |
| `search`        | Searches for packages matching given criteria.                              |
| `info`          | Displays detailed information about specified packages.                     |
| `refresh`       | Refreshes the repository metadata.                                          |
| `list-updates`  | Lists all packages with available updates.                                  |
| `repolist`      | Displays all defined repositories.                                          |
| `addrepo`       | Adds a new repository.                                                      |
| `removerepo`    | Removes a specified repository.                                             |

## Usage Examples

### Install a Package
```bash
zypper install PACKAGE_NAME
```

### Remove a Package
```bash
zypper remove PACKAGE_NAME
```

### Update System Packages
```bash
zypper update
```

### Search for a Package
```bash
zypper search KEYWORD
```

### Get Info on a Package
```bash
zypper info PACKAGE_NAME
```

### Refresh Repository Data
```bash
zypper refresh
```

### List Repositories
```bash
zypper repolist
```

### Add a New Repository
```bash
zypper addrepo URL REPO_NAME
```

### Remove a Repository
```bash
zypper removerepo REPO_NAME
```

## Cheat Sheet

```plaintext
# Install a package
zypper in PACKAGE_NAME

# Remove a package
zypper rm PACKAGE_NAME

# Update system
zypper up

# Search for a package
zypper se KEYWORD

# Refresh repositories
zypper ref
```
