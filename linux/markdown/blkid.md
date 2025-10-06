# `blkid` Command

The `blkid` command in Linux is used to retrieve information about block devices, primarily focusing on attributes like UUID and filesystem type.

## Common Options

| Option  | Description                                   |
|---------|-----------------------------------------------|
| `-c`    | Specify a cache file (default is `/etc/blkid.tab`). |
| `-o`    | Define the output format (e.g., `full`, `value`, `list`). |
| `-s`    | Show specific tags (e.g., `UUID`, `TYPE`).    |
| `-t`    | Filter devices by specific tag=value pairs.   |
| `-v`    | Enable verbose output.                        |
| `-p`    | Probe a specific block device only.           |

## Usage Examples

### List All Block Devices

```bash
blkid
```

### Filter by Filesystem Type

```bash
blkid -t TYPE=ext4
```

### Show Only UUIDs

```bash
blkid -s UUID
```

### Specify Output Format

```bash
blkid -o list
```

### Probe a Specific Device

```bash
blkid -p /dev/sda1
```

## Cheat Sheet

```plaintext
# List all block devices
blkid

# Display UUIDs only
blkid -s UUID

# Filter by filesystem type
blkid -t TYPE=ext4

# Use list output format
blkid -o list

# Probe a specific device
blkid -p /dev/sda1
```
