# Deja Dup Command

`deja-dup` is a tool for backing up files within a Linux environment. It provides a simple way to perform regular backups and restore files when needed.

## Common Options

| Option           | Explanation                                  |
|------------------|----------------------------------------------|
| `--backup`       | Start a backup process.                      |
| `--restore`      | Restore files from the last backup.          |
| `--restore-missing FILE` | Restore a missing file.              |
| `--list`         | Show files in the last backup.               |
| `--version`      | Display the version information.             |
| `--help`         | Display help for the command.                |

## Usage Examples

### Starting a Backup
To start a backup of your files configured through the GUI:

```bash
deja-dup --backup
```

### Restoring the Latest Backup
Restore all files from the most recent backup:

```bash
deja-dup --restore
```

### Restoring a Specific Missing File
Restore a specific missing file:

```bash
deja-dup --restore-missing ~/Documents/example.txt
```

### Listing Files in the Last Backup
List all files in the latest backup:

```bash
deja-dup --list
```

## Cheat Sheet

```plaintext
deja-dup --backup          # Start backup
deja-dup --restore         # Restore from latest backup
deja-dup --restore-missing FILE  # Restore a specific file
deja-dup --list            # List files in the last backup
```
