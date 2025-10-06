# Timeshift Command Overview

`timeshift` is a powerful backup and restore tool for Linux systems, primarily used to create and manage system snapshots. It helps in restoring your system to a previous state in case of system failure or errors.

## Common Options

| Option          | Description                                           |
|-----------------|-------------------------------------------------------|
| `--create`      | Create a new snapshot.                                |
| `--restore`     | Restore from a specified snapshot.                    |
| `--list`        | List all available snapshots.                         |
| `--check`       | Check current system for snapshots.                   |
| `--delete`      | Delete a specified snapshot.                          |
| `--help`        | Display help information for the command.             |
| `--backup-device <device>` | Specify the backup device for snapshots. |

## Usage Examples

### Create a Snapshot

```bash
sudo timeshift --create
```

### Restore a Snapshot

```bash
sudo timeshift --restore --snapshot '2023-10-01_12-00-00'
```

### List Available Snapshots

```bash
timeshift --list
```

### Delete a Snapshot

```bash
sudo timeshift --delete --snapshot '2023-10-01_12-00-00'
```

### Check System for Snapshots

```bash
timeshift --check
```

## Cheat Sheet

```plaintext
# Create a new snapshot
sudo timeshift --create

# Restore a specific snapshot
sudo timeshift --restore --snapshot '<snapshot-name>'

# List snapshots
timeshift --list

# Delete a specific snapshot
sudo timeshift --delete --snapshot '<snapshot-name>'

# Check system for snapshots
timeshift --check
```
