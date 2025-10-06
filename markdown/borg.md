# Borg Command in Linux

## Description

`borg` is a powerful deduplicating backup tool that allows you to efficiently manage filesystem data. It focuses on backup and restoration with features like compression, encryption, and remote repository support.

## Common Options

| Option            | Description                                               |
|-------------------|-----------------------------------------------------------|
| `init`            | Initialize a new backup repository.                       |
| `create`          | Create a new backup archive in the repository.            |
| `extract`         | Extract files from an archive.                            |
| `list`            | List archives or archive contents.                        |
| `info`            | Display detailed info about archives/repository.          |
| `prune`           | Delete old archives according to a retention policy.      |
| `check`           | Verify repository consistency and integrity.              |
| `key`             | Manage repository encryption keys.                        |
| `mount`           | Mount an archive as a FUSE filesystem.                    |

## Usage Examples

### Initialize a Repository

```bash
borg init --encryption=repokey /path/to/repo
```

### Create a Backup

```bash
borg create /path/to/repo::archive-name /path/to/directory
```

### Extract Files

```bash
borg extract /path/to/repo::archive-name /path/to/extract
```

### List Archives

```bash
borg list /path/to/repo
```

### Prune Old Backups

```bash
borg prune -v --list /path/to/repo --keep-daily=7 --keep-weekly=4 --keep-monthly=6
```

## Cheat Sheet

```plaintext
borg init --encryption=repokey /repo     # Initialize
borg create /repo::arch-name /dir        # Create archive
borg extract /repo::arch-name /dest      # Extract archive
borg list /repo                          # List archives
borg prune -v --list /repo --keep-daily=7 --keep-weekly=4 --keep-monthly=6  # Prune
```
