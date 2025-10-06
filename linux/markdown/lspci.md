# `lspci` Command Overview

`lspci` is a command-line utility in Linux used to display detailed information about all PCI buses and devices in the system. This tool is essential for diagnosing hardware issues and listing hardware devices.

## Common Options

| Option        | Description                                       |
|---------------|---------------------------------------------------|
| `-v`          | Verbose output; provides more detailed information about each device. |
| `-vv`         | Very verbose output; displays even more detailed information. |
| `-k`          | Show kernel drivers handling each device.         |
| `-t`          | Show a tree view of the devices.                  |
| `-nn`         | Show both numeric and readable form of Vendor and Device names. |
| `-s <slot>`   | Show information about the device in a specific slot. |
| `-d <vendor>:<device>` | Show only devices with a specified vendor and device ID. |

## Usage Examples

### Example 1: Basic Device Information

Get a quick list of all PCI devices:

```bash
lspci
```

### Example 2: Detailed Information

Include verbose details for troubleshooting:

```bash
lspci -v
```

### Example 3: Show Kernel Drivers

List PCI devices with their kernel drivers:

```bash
lspci -k
```

### Example 4: Tree View

Visualize the hierarchy of PCI devices:

```bash
lspci -t
```

### Example 5: Filter by Vendor and Device ID

Find devices from a specific vendor:

```bash
lspci -d 8086:
```

## Cheat Sheet

```markdown
# List all PCI devices
lspci

# Verbose information
lspci -v

# Show kernel drivers
lspci -k

# Tree view
lspci -t

# Specify vendor and device
lspci -d <vendor>:<device>
```
