# Snapshot Command in Linux

The `snapshot` command is not a standard Linux utility. However, in some contexts, it might refer to custom scripts or software used for filesystem snapshots. These snapshots provide a way to capture the state of filesystems at a specific point in time, often used for backups or system recovery.

Below, I'll provide a general guide assuming `snapshot` is a tool related to any similar utility or context where snapshots are used.

## Common Options

| Option             | Description                                        |
|--------------------|----------------------------------------------------|
| `-c, --create`     | Create a new snapshot.                             |
| `-l, --list`       | List available snapshots.                          |
| `-r, --restore`    | Restore to a specified snapshot.                   |
| `-d, --delete`     | Delete a specified snapshot.                       |
| `-n, --name`       | Specify the name for the snapshot.                 |
| `-s, --schedule`   | Schedule regular snapshots.                        |

## Usage Examples

### Create a New Snapshot
```bash
snapshot --create --name daily-backup
```

### List Available Snapshots
```bash
snapshot --list
```

### Restore a Snapshot
```bash
snapshot --restore --name daily-backup
```

### Delete a Snapshot
```bash
snapshot --delete --name old-backup
```

### Schedule Regular Snapshots
```bash
snapshot --schedule "0 2 * * *" --name nightly-backup
```

## Cheat Sheet

```plaintext
# Create a snapshot
snapshot -c -n <snapshot_name>

# List snapshots
snapshot -l

# Restore a snapshot
snapshot -r -n <snapshot_name>

# Delete a snapshot
snapshot -d -n <snapshot_name>

# Schedule snapshots
snapshot -s "<cron_syntax>" -n <snapshot_name>
```
