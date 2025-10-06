# Restore-SqlDatabase Command

`Restore-SqlDatabase` is a PowerShell cmdlet used to restore SQL Server databases from a backup. It offers flexibility in handling various backup types and options to customize the restore process.

## Common Options

| Option                      | Description                                                                 |
|-----------------------------|-----------------------------------------------------------------------------|
| `-ServerInstance`           | Specifies the SQL Server instance name.                                     |
| `-Database`                 | Defines the name of the database to be restored.                            |
| `-BackupFile`               | Specifies the path to the backup file.                                      |
| `-NoRecovery`               | Leaves the database in restoring state, allowing further logs to be applied.|
| `-BackupAction`             | Indicates the type of restore action (`Database`, `Log`, etc.).             |
| `-RestoreAction`            | Defines the restore action (`Database`, `File`, etc.).                      |
| `-ReplaceDatabase`          | Replaces the existing database.                                             |
| `-RelocateFile`             | Relocates the database files to a new file path.                            |

## Usage Examples

### Restore a Full Database Backup

```powershell
Restore-SqlDatabase -ServerInstance "ServerName\InstanceName" -Database "MyDatabase" -BackupFile "C:\Backups\MyDatabase.bak" -ReplaceDatabase
```

### Restore a Database and Leave it in a Restoring State

```powershell
Restore-SqlDatabase -ServerInstance "ServerName\InstanceName" -Database "MyDatabase" -BackupFile "C:\Backups\MyDatabase.bak" -NoRecovery
```

### Restore and Relocate Database Files

```powershell
Restore-SqlDatabase -ServerInstance "ServerName\InstanceName" -Database "MyDatabase" -BackupFile "C:\Backups\MyDatabase.bak" -RelocateFile @{"MyDatabase_Data"="D:\Data\MyDatabase.mdf"; "MyDatabase_Log"="E:\Logs\MyDatabase.ldf"}
```

## Cheat Sheet

- **Full Restore**:
  ```powershell
  Restore-SqlDatabase -S "Server\Instance" -D "DB" -BackupFile "Path.bak" -ReplaceDatabase
  ```

- **With No Recovery**:
  ```powershell
  Restore-SqlDatabase -S "Server\Instance" -D "DB" -BackupFile "Path.bak" -NoRecovery
  ```

- **Relocate Files**:
  ```powershell
  Restore-SqlDatabase -S "Server\Instance" -D "DB" -BackupFile "Path.bak" -RelocateFile @{"Data"="NewPath.mdf"; "Log"="NewPath.ldf"}
  ```

Use this guide as a quick reference to efficiently use the `Restore-SqlDatabase` cmdlet in various scenarios.
