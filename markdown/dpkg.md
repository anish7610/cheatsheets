# `dpkg` Command in Linux

## Description

`dpkg` is a low-level package management system for Debian-based systems. It is used to install, remove, and manage `.deb` packages.

## Common Options

| Option             | Explanation                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| `-i`, `--install`  | Install a package.                                                          |
| `-r`, `--remove`   | Remove a package, keeping configuration files.                              |
| `-P`, `--purge`    | Remove a package, including configuration files.                            |
| `-l`, `--list`     | List all installed packages.                                                |
| `-L`, `--listfiles`| List files installed by the package.                                        |
| `-s`, `--status`   | Display the status of a package.                                            |
| `-S`, `--search`   | Search for a file installed by a package.                                   |
| `--configure`      | Reconfigure an unpacked package.                                            |
| `--audit`          | Show packages that require installation, removal, or configuration actions. |

## Usage Examples

### Install a Package
```bash
sudo dpkg -i package_name.deb
```

### Remove a Package (Keep Configuration Files)
```bash
sudo dpkg -r package_name
```

### Completely Remove a Package (Including Configuration Files)
```bash
sudo dpkg -P package_name
```

### List All Installed Packages
```bash
dpkg -l
```

### List Files Installed by a Package
```bash
dpkg -L package_name
```

### Display Status of a Specific Package
```bash
dpkg -s package_name
```

### Search for a File Installed by a Package
```bash
dpkg -S /path/to/file
```

## Cheat Sheet

```plaintext
Install:   sudo dpkg -i [package.deb]
Remove:    sudo dpkg -r [package]
Purge:     sudo dpkg -P [package]
List:      dpkg -l
Files:     dpkg -L [package]
Status:    dpkg -s [package]
Search:    dpkg -S [file]
```
