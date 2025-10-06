# `restore` Command in Linux

`restore` is used to restore files from backups created by the `dump` command. It reads tape volumes, or files saved by `dump`, and restores them to a specified directory.

## Common Options

| Option      | Explanation                                                            |
|-------------|------------------------------------------------------------------------|
| `-f device` | Specifies the archive file or device from which to restore.            |
| `-r`        | Restores the entire backup. Useful for complete restoration.           |
| `-i`        | Interactive mode. Allows selective file restoration.                   |
| `-t`        | Lists the files and directories in the backup without restoring them.  |
| `-v`        | Verbose output. Displays detailed operations performed by `restore`.   |
| `-x`        | Extracts specific files or directories from the backup.                |
| `-d`        | Debug mode. Provides detailed debugging information.                   |

## Usage Examples

### Restore Entire Backup

```bash
restore -r -f /dev/sdX1
```

This command restores an entire backup from the specified device `/dev/sdX1`.

### Interactive File Restore

```bash
restore -i -f /backup/archive.bak
```

Enters interactive mode, allowing you to choose files to restore from `archive.bak`.

### List Contents of a Backup

```bash
restore -t -f /backup/archive.bak
```

Lists the contents of `archive.bak` without restoring any files.

### Restore Specific Files

```bash
restore -x -f /backup/archive.bak ./documents/report.txt
```

Extracts `report.txt` from `archive.bak` to the current directory.

## Cheat Sheet

```plaintext
# Restore full backup
restore -r -f /dev/sdX1

# Interactive restore
restore -i -f archive.bak

# List backup contents
restore -t -f archive.bak

# Extract specific files
restore -x -f archive.bak ./file_path
```

Use this concise guide to quickly reference the key functionalities of the `restore` command in Linux.
