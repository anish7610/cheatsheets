# `dd` Command Overview

The `dd` command in Linux is used for converting and copying files. It's powerful for tasks like creating disk images, cloning drives, and transferring data between devices.

## Common Options

| Option  | Description                                      |
|---------|--------------------------------------------------|
| `if=`   | Input file or device source                      |
| `of=`   | Output file or device destination                |
| `bs=`   | Block size for read/write operations             |
| `count=`| Number of blocks to copy                         |
| `status=`| Display progress during execution               |
| `conv=` | Conversion options (e.g., `noerror`, `sync`)     |

## Usage Examples

### Create a Disk Image

Create an image of a disk or partition:

```bash
dd if=/dev/sdX of=/path/to/disk.img bs=4M status=progress
```

### Restore a Disk Image

Write an image to a disk or partition:

```bash
dd if=/path/to/disk.img of=/dev/sdX bs=4M status=progress
```

### Wipe a Disk

Fill a disk with zeros (all data will be erased):

```bash
dd if=/dev/zero of=/dev/sdX bs=1M status=progress
```

### Create a Bootable USB Drive

Transfer an ISO file to a USB drive:

```bash
dd if=/path/to/file.iso of=/dev/sdX bs=4M status=progress
```

## Cheat Sheet

```plaintext
# Copy disk or partition
dd if=/dev/sdX of=/path/to/disk.img bs=4M status=progress

# Write image to disk
dd if=/path/to/disk.img of=/dev/sdX bs=4M status=progress

# Erase disk with zeros
dd if=/dev/zero of=/dev/sdX bs=1M status=progress

# Create bootable USB
dd if=/path/to/file.iso of=/dev/sdX bs=4M status=progress
```

> **Note:** Always ensure the correct `if` and `of` paths to avoid data loss. Use the `lsblk` command to list devices and confirm paths.
