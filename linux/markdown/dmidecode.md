# `dmidecode` Command Overview

`dmidecode` is a command-line tool for Linux that provides detailed information about the system's hardware components by reading the DMI (Desktop Management Interface) table. It is primarily used for retrieving information like BIOS version, serial numbers, and memory configuration without needing to manually inspect the hardware.

## Common Options

| Option            | Description                                              |
|-------------------|----------------------------------------------------------|
| `-t, --type TYPE` | Display only the entries of a specific type.             |
| `-q, --quiet`     | Suppress output of irrelevant information.               |
| `-s, --string`    | Only print the specified DMI string.                     |
| `-u, --dump-bin`  | Dump the DMI data to a binary file.                      |
| `-h, --help`      | Display help and exit.                                   |
| `-V, --version`   | Output version information and exit.                     |

## Usage Examples

### Display BIOS Information
```bash
sudo dmidecode -t bios
```

### Show System Information
```bash
sudo dmidecode -t system
```

### Extract System Serial Number
```bash
sudo dmidecode -s system-serial-number
```

### List All Processor Information
```bash
sudo dmidecode -t processor
```

## Cheat Sheet

```bash
# BIOS information
sudo dmidecode -t bios

# Processor details
sudo dmidecode -t processor

# System serial number
sudo dmidecode -s system-serial-number

# Complete system information
sudo dmidecode -t system
```
