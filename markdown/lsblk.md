## `lsblk` Command Overview

`lsblk` is a command-line utility in Linux used to list information about all available or specified block devices. It provides a tree view of devices, showing their mount points, sizes, and more, which is helpful for managing storage.

## Common Options

| Option | Description                               |
|--------|-------------------------------------------|
| `-a`   | List all devices, including empty and RAM disks. |
| `-d`   | Output only block devices, not partitions. |
| `-f`   | Display file system (FS) information.      |
| `-l`   | Use a list format instead of a tree format.|
| `-n`   | Omit the header row.                       |
| `-o`   | Specify output columns.                    |
| `-p`   | Include partition names with full paths.   |
| `-r`   | Print in raw format without tree view.     |
| `-t`   | Display topology information.              |
| `-J`   | Print the output in JSON format.           |

## Usage Examples

### List all block devices
```bash
lsblk
```

### List only block devices without partition details
```bash
lsblk -d
```

### Display file system information
```bash
lsblk -f
```

### Use list format instead of tree format
```bash
lsblk -l
```

### Display detailed information with specific columns
```bash
lsblk -o NAME,SIZE,TYPE,MOUNTPOINT
```

### Display information in JSON format
```bash
lsblk -J
```

### Display all devices, including empty ones
```bash
lsblk -a
```

## Cheat Sheet

```plaintext
lsblk         # List block devices in tree format
lsblk -d      # Device info only, no partitions
lsblk -f      # Include filesystem info
lsblk -l      # List format output
lsblk -o COLS # Custom columns: NAME,SIZE
```
