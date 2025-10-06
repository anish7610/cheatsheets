# Windows Backup Command

The `Windows Backup` command, also known as `wbadmin`, is a command-line utility in Windows that allows users to create, manage, and restore backups.

## Common Options

| Option               | Explanation                                        |
|----------------------|----------------------------------------------------|
| `start backup`       | Initiates a backup operation.                      |
| `stop job`           | Stops the currently running backup or recovery.    |
| `get versions`       | Lists available backups that can be restored.      |
| `start recovery`     | Initiates a recovery using a specified backup.     |
| `enable backup`      | Configures a scheduled daily backup.               |
| `disable backup`     | Disables the scheduled daily backup.               |

## Usage Examples

- **Create a Backup**:
  ```bash
  wbadmin start backup -backupTarget:D: -include:C:
  ```

- **Stop an Ongoing Job**:
  ```bash
  wbadmin stop job
  ```

- **List Available Backups**:
  ```bash
  wbadmin get versions
  ```

- **Start Recovery from a Backup**:
  ```bash
  wbadmin start recovery -version:03/21/2023-18:35
  ```

- **Enable Scheduled Daily Backup**:
  ```bash
  wbadmin enable backup -addtarget:\\server\share -schedule:12:00
  ```

## Cheat Sheet

```plaintext
# Start a backup
wbadmin start backup -backupTarget:<Drive> -include:<Volumes>

# Stop a job
wbadmin stop job

# List backups
wbadmin get versions

# Start recovery
wbadmin start recovery -version:<Date-Time>

# Enable scheduled backup
wbadmin enable backup -addtarget:<Path> -schedule:<Time>
```

Note: Replace placeholders like `<Drive>`, `<Volumes>`, `<Date-Time>`, `<Path>`, and `<Time>` with actual values.
