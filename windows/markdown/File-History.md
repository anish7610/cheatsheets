# Windows File History Command

File History is a backup utility in Windows that allows users to automatically back up and restore versions of files stored in designated folders. It primarily targets Libraries, Desktop, Contacts, and Favorites. It creates incremental backups of files in user-specified locations.

## Common Options

| Option                | Explanation                                                    |
|-----------------------|----------------------------------------------------------------|
| `-backuptarget`       | Specifies a location for backups.                             |
| `-archive`            | Marks a backup as an archive version.                         |
| `-cleanup`            | Deletes older backup versions, based on specified criteria.   |
| `-quiet`              | Runs the command without user interaction or prompts.         |
| `-monitor`            | Monitors the File History configuration and status.           |

## Usage Examples

### Enable File History

```bash
FileHistory.exe -enable
```

Enable File History on your device.

### Set Backup Location

```bash
FileHistory.exe -setbackuplocation D:\Backup
```

Set `D:\Backup` as the target location for backups.

### Run in Quiet Mode

```bash
FileHistory.exe -backupnow -quiet
```

Perform a backup operation without prompts or notifications.

### Clean Up Old Backups

```bash
FileHistory.exe -cleanup
```

Delete old versions based on the defined backup policy.

## Cheat Sheet

```plaintext
Enable:      FileHistory.exe -enable
Set location: FileHistory.exe -setbackuplocation [path]
Backup now:  FileHistory.exe -backupnow [-quiet]
Cleanup:     FileHistory.exe -cleanup
Monitor:     FileHistory.exe -monitor
```
