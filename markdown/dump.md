# `dump` Command in Linux

## Description

The `dump` command is used to back up file systems on Linux. It is specifically designed for ext2/ext3 file systems and creates backups that can be restored using the `restore` command.

## Common Options

| Option | Description                                      |
|--------|--------------------------------------------------|
| `-0` to `-9` | Specifies the backup level (0 for full, 1-9 for incremental). |
| `-u`  | Update `/etc/dumpdates` after a successful dump.  |
| `-f`  | Defines the output file or device for the backup. |
| `-B`  | Sets the size of the output file in kilobytes.    |
| `-j`  | Enables bzip2 compression of the dump.            |
| `-W`  | Outputs what file systems need to be dumped.      |

## Usage Examples

### Full Backup of a File System
```bash
dump -0u -f /backup/home.dump /dev/sda1
```

### Incremental Backup
```bash
dump -1u -f /backup/home.incremental.dump /dev/sda1
```

### Compressed Full Backup
```bash
dump -0uj -f /backup/home.bz2.dump /dev/sda1
```

### Check File Systems to be Dumped
```bash
dump -W
```

## Cheat Sheet

```plaintext
Full backup:      dump -0u -f /path/to/backup.dump /dev/sdXN
Incremental:      dump -1u -f /path/to/backup.dump /dev/sdXN
Compressed:       dump -0uj -f /path/to/backup.bz2.dump /dev/sdXN
Check dumps:      dump -W
```

Replace `/dev/sdXN` with the appropriate device identifier for your system.
