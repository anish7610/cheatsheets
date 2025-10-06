# `fsarchiver` Command Overview

`fsarchiver` is a flexible tool used for file system backup and restoration. It allows you to save the contents of a file system to a compressed archive file.

## Common Options

| Option          | Explanation                                                                 |
|-----------------|-----------------------------------------------------------------------------|
| `-a, --autosave-log` | Automatically save log files in `/var/log/fsarchiver/`.                  |
| `-c, --compress` | Set compression level (0-9). Higher levels result in smaller files.        |
| `-d, --directory` | Specify a directory to include in the archive.                           |
| `-e, --exclude`  | Exclude specified files or directories from the backup.                   |
| `-j, --jobs`     | Number of parallel compression jobs. Adjust to utilize multi-core CPUs.   |
| `-z, --chunksize`| Set size of each chunk (default is 64 MiB).                               |
| `-v, --verbose`  | Output detailed operation logs to the console.                            |
| `-S, --split`    | Split archive into smaller fixed-size files (e.g., 700m for CDs).         |

## Usage Examples

### Backup a File System
Creating an archive of a file system `/dev/sda1`:
```bash
fsarchiver savefs /path/to/backup.fsa /dev/sda1
```

### Restore a File System
Restoring from an archive to a file system `/dev/sda1`:
```bash
fsarchiver restfs /path/to/backup.fsa id=0,dest=/dev/sda1
```

### Backup with Compression
Backup using maximum compression:
```bash
fsarchiver -c9 savefs /path/to/backup.fsa /dev/sda1
```

### Exclude Specific Directories
Exclude `/tmp` directory from the backup:
```bash
fsarchiver savefs /path/to/backup.fsa /dev/sda1 -e /tmp
```

### Split Archive into Parts
Split the archive into 2GB parts:
```bash
fsarchiver -S2G savefs /path/to/backup.fsa /dev/sda1
```

## Cheat Sheet

```plaintext
fsarchiver savefs <archive> <device> [options]
fsarchiver restfs <archive> id=0,dest=<device> [options]

Options:
  -cN    Compression level (N = 0-9)
  -e     Exclude files/dirs
  -S<N>  Split size (e.g., 700m, 1G)
```
