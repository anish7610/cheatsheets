# `df` Command in Linux

## Description

The `df` (disk free) command is used to report the amount of available disk space on file systems. It provides a quick view of disk usage, making it useful for monitoring storage needs.

## Common Options

| Option       | Description                                    |
|--------------|------------------------------------------------|
| `-h`         | Human-readable format (e.g., 1K, 234M, 2G)     |
| `-a`         | Include all file systems                       |
| `-T`         | Display file system type                       |
| `-i`         | Show inode usage instead of block usage        |
| `-t <type>`  | Limit output to file systems of specified type |
| `-x <type>`  | Exclude file systems of specified type         |
| `--total`    | Show a total at the bottom of the report       |

## Usage Examples

### Basic Usage
```bash
df
```

### Human-Readable Format
```bash
df -h
```

### Include All File Systems
```bash
df -a
```

### Show File System Types
```bash
df -T
```

### Show Inode Usage
```bash
df -i
```

### Limit to Specific File System Type (e.g., ext4)
```bash
df -t ext4
```

### Exclude Specific File System Type (e.g., tmpfs)
```bash
df -x tmpfs
```

### Show Total Disk Usage
```bash
df --total
```

## Cheat Sheet

```plaintext
df          # Basic disk usage
df -h       # Human-readable format
df -T       # Include file system types
df -i       # Show inode usage
df -t ext4  # Only ext4 file systems
df -x tmpfs # Exclude tmpfs file systems
```

This guide provides a straightforward approach to using `df` effectively for everyday disk monitoring tasks.
