# Duplicity Command

Duplicity is a command-line backup tool for Linux that enables encrypted, incremental backups. It supports various backend storage options such as local files, FTP, SSH, Amazon S3, Google Drive, and more.

## Common Options

| Option               | Description                                                  |
|----------------------|--------------------------------------------------------------|
| `full`               | Perform a full backup.                                       |
| `incremental`        | Create an incremental backup.                                |
| `restore`            | Restore files from a backup.                                 |
| `collection-status`  | Show the status of the backup sets.                          |
| `remove-older-than X`| Delete backups older than a specified time (X).              |
| `--encrypt-key <key>`| Use GPG encryption with the given key ID.                    |
| `--sign-key <key>`   | Use the specified key ID to sign backups.                    |
| `--verbosity <level>`| Set the level of verbosity (0 to 9).                         |

## Usage Examples

### Full Backup to Remote Server via SSH

```bash
duplicity full /home/user ssh://user@remote.server.com/backup-dir
```

### Incremental Backup to Amazon S3

```bash
duplicity incremental /home/user s3://bucket-name/backup-dir
```

### Restore Backup from Local Directory

```bash
duplicity restore file:///home/user/backup-dir /home/user/restore-dir
```

### Delete Backups Older than 30 Days

```bash
duplicity remove-older-than 30D --force file:///home/user/backup-dir
```

### Check Backup Collection Status

```bash
duplicity collection-status file:///home/user/backup-dir
```

## Cheat Sheet

```plaintext
# Full Backup
duplicity full <source> <destination>

# Incremental Backup
duplicity incremental <source> <destination>

# Restore
duplicity restore <backup_location> <restore_location>

# Remove Old Backups
duplicity remove-older-than <time> --force <backup_location>

# Backup Status
duplicity collection-status <backup_location>
```

Remember to replace placeholders like `<source>`, `<destination>`, `<backup_location>`, and `<time>` with your actual paths and desired time duration (e.g., `30D` for 30 days).
