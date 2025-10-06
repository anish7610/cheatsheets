## `wbadmin` Command Overview

`wbadmin` is a command-line utility for managing backup and recovery operations on Windows. It allows users to create, manage, and restore backups of the system and data.

## Common Options

| Option                | Description                                           |
|-----------------------|-------------------------------------------------------|
| `start backup`        | Initiates a backup operation.                         |
| `stop job`            | Halts a running backup or recovery operation.         |
| `get versions`        | Lists details of backups available.                   |
| `get items`           | Lists files or applications in a backup.              |
| `delete systemstatebackup` | Deletes system state backups.                    |
| `start recovery`      | Starts a recovery operation using a specified version.|
| `enable backup`       | Enables a scheduled daily backup.                     |
| `disable backup`      | Disables the scheduled backups.                       |

## Usage Examples

### Start a Backup

```bash
wbadmin start backup -backupTarget:D: -include:C: -quiet
```

Creates a backup of the C: drive to the D: drive without prompts.

### Stop a Running Job

```bash
wbadmin stop job
```

Stops an ongoing backup or recovery process.

### List Available Backups

```bash
wbadmin get versions
```

Displays all available backup versions.

### Recover Files from a Backup

```bash
wbadmin start recovery -version:03/15/2023-09:00 -itemType:File -items:C:\Docs -recoveryTarget:C:\Recovery
```

Restores files under `C:\Docs` from a specific backup version to `C:\Recovery`.

### Enable Scheduled Backup

```bash
wbadmin enable backup -addtarget:\\BackupServer\Backups
```

Enables a daily scheduled backup to a network location.

## Cheat Sheet

```plaintext
start backup -backupTarget:<target> -include:<items> -quiet
stop job
get versions
start recovery -version:<date-time> -itemType:<type> -items:<items> -recoveryTarget:<path>
```

Ensure you have administrative privileges to run `wbadmin` commands.
