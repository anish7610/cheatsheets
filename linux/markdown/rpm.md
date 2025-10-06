# RPM Command Overview

`rpm` (Red Hat Package Manager) is a command-line utility for managing packages on RPM-based Linux distributions, such as RHEL, CentOS, and Fedora. It allows users to install, update, remove, and query software packages.

## Common Options

| Option            | Description                                          |
|-------------------|------------------------------------------------------|
| `-i`              | Install a new package                                |
| `-U`              | Upgrade an existing package                          |
| `-e`              | Erase (remove) a package                             |
| `-q`              | Query a package                                      |
| `-qa`             | Query all installed packages                         |
| `-ql`             | List files installed by a package                    |
| `-qi`             | Display package information                          |
| `-qc`             | List configuration files from a package              |
| `-V`              | Verify a package                                     |
| `--test`          | Test transactions without making any changes         |

## Usage Examples

### Install a Package
```bash
rpm -i package.rpm
```

### Upgrade a Package
```bash
rpm -U package.rpm
```

### Remove a Package
```bash
rpm -e package-name
```

### Query a Package
```bash
rpm -q package-name
```

### List All Installed Packages
```bash
rpm -qa
```

### List Files of a Package
```bash
rpm -ql package-name
```

### Display Information of a Package
```bash
rpm -qi package-name
```

### Verify a Package
```bash
rpm -V package-name
```

## Cheat Sheet

```plaintext
Install:    rpm -i <package.rpm>
Upgrade:    rpm -U <package.rpm>
Remove:     rpm -e <package-name>
Query:      rpm -q <package-name>
List All:   rpm -qa
List Files: rpm -ql <package-name>
Info:       rpm -qi <package-name>
Verify:     rpm -V <package-name>
```
