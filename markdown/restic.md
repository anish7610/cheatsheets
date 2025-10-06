# `restic` Command Overview

`restic` is a fast, secure, and efficient backup program designed to handle large amounts of data. It supports deduplication, encryption, and various storage backends.

## Common Options

| Option                  | Description                                     |
|-------------------------|-------------------------------------------------|
| `backup <paths>`        | Creates a backup of the specified paths.        |
| `restore <snapshot>`    | Restores files from a snapshot.                 |
| `snapshots`             | Lists all available snapshots.                  |
| `check`                 | Verifies the integrity of the repository.       |
| `init`                  | Initializes a new repository.                   |
| `forget`                | Removes snapshots according to a policy.        |
| `prune`                 | Cleans up the repository and removes unneeded data. |
| `mount <path>`          | Mounts the repository at a given path.          |
| `unlock`                | Removes stale locks in the repository.          |
| `stats`                 | Displays statistics about the repository.       |

## Usage Examples

### Initialize a Repository

```bash
restic init --repo /path/to/repo
```

### Backup Files

```bash
restic backup /home/user/documents --repo /path/to/repo
```

### List Snapshots

```bash
restic snapshots --repo /path/to/repo
```

### Restore a Snapshot

```bash
restic restore <snapshot-id> --target /path/to/restore --repo /path/to/repo
```

### Check Repository Integrity

```bash
restic check --repo /path/to/repo
```

### Forget Old Snapshots

```bash
restic forget --keep-last 3 --prune --repo /path/to/repo
```

## Cheat Sheet

```plaintext
restic init --repo /path/to/repo
restic backup /path/to/data --repo /path/to/repo
restic restore <id> --target /path/to/target --repo /path/to/repo
restic snapshots --repo /path/to/repo
restic check --repo /path/to/repo
restic forget --keep-last n --prune --repo /path/to/repo
```
