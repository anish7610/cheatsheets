# Linux `du` Command

The `du` (disk usage) command estimates and displays the amount of disk space used by files and directories.

## Common Options

| Option         | Description                                          |
|----------------|------------------------------------------------------|
| `-a`           | Show sizes of individual files as well as directories. |
| `-h`           | Display sizes in human-readable format (e.g., KB, MB). |
| `-s`           | Show only the total size of each argument.           |
| `-c`           | Produce a grand total.                               |
| `-d N`         | Limit the depth of directory traversal to N levels.  |
| `--max-depth=N`| Same as `-d N`.                                      |
| `--exclude=PATTERN` | Exclude files matching PATTERN.                |

## Usage Examples

### Display Disk Usage of a Directory in Human-Readable Format

```bash
du -h /path/to/directory
```

### Show Total Disk Usage of a Directory

```bash
du -sh /path/to/directory
```

### List Disk Usage of All Files and Directories

```bash
du -ah /path/to/directory
```

### Limit Display to One Level Deep

```bash
du -h --max-depth=1 /path/to/directory
```

### Show Disk Usage Excluding Certain Files

```bash
du -h --exclude='*.log' /path/to/directory
```

### Combine Total of Multiple Directories

```bash
du -ch /dir1 /dir2
```

## Cheat Sheet

```bash
du -h       # Disk usage in human-readable format
du -sh      # Total size for a directory
du -ah      # Include files, human-readable
du -h -d 1  # Limit depth to 1
du -h --exclude='*.log'  # Exclude patterns
```
