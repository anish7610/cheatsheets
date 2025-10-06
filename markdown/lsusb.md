# `lsusb` Command Overview

The `lsusb` command lists all USB devices connected to a Linux system. It provides details about each device, such as the manufacturer, product ID, and bus number.

## Common Options

| Option | Description                                                                 |
|--------|-----------------------------------------------------------------------------|
| `-v`   | Display detailed information about each USB device.                         |
| `-s`   | Restrict results to a specific device by bus and device number (e.g., `-s 001:002`). |
| `-d`   | Show information about a specific vendor and product ID (e.g., `-d 12d1:1052`).     |
| `-t`   | Display the USB device hierarchy as a tree.                                 |
| `-V`   | Show version information for `lsusb`.                                       |

## Usage Examples

### List All USB Devices

```bash
lsusb
```

### Show Detailed Information

```bash
lsusb -v
```

### List Devices on a Specific Bus and Device Number

```bash
lsusb -s 001:003
```

### Filter by Vendor and Product ID

```bash
lsusb -d 12d1:1052
```

### Display USB Device Tree

```bash
lsusb -t
```

## Cheat Sheet

```markdown
- `lsusb`                 # List USB devices
- `lsusb -v`              # Verbose output
- `lsusb -s <bus>:<device>` # Specify bus and device
- `lsusb -d <vendor>:<product>` # Filter by vendor/product
- `lsusb -t`              # Device tree view
```
