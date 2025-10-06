# Get-SqlDatabaseBackup Command

`Get-SqlDatabaseBackup` is a PowerShell command used to retrieve information about the backups of SQL Server databases. It is part of the SQLServer module in PowerShell, providing insights into backup history, types, and details.

## Common Options

| Option                | Explanation                                                  |
|-----------------------|--------------------------------------------------------------|
| `-ServerInstance`     | Specifies the SQL Server instance to connect to.             |
| `-Database`           | Specifies the name of the database to query backup history.  |
| `-Last`               | Retrieves only the most recent backup information.           |
| `-BackupActionType`   | Filters results by backup type (Full, Differential, Log).    |
| `-Path`               | Outputs the backup information to a specified file path.     |

## Usage Examples

### Retrieve Recent Backups for a Database

```powershell
Get-SqlDatabaseBackup -ServerInstance "MyServer" -Database "MyDatabase" -Last
```

### List All Full Backups for a Database

```powershell
Get-SqlDatabaseBackup -ServerInstance "MyServer" -Database "MyDatabase" -BackupActionType Full
```

### Save Backup Information to a File

```powershell
Get-SqlDatabaseBackup -ServerInstance "MyServer" -Database "MyDatabase" -Path "C:\backups\backup_info.txt"
```

## Cheat Sheet

```plaintext
# Basic backup retrieval
Get-SqlDatabaseBackup -ServerInstance "Server" -Database "DB"

# Latest backup only
Get-SqlDatabaseBackup -ServerInstance "Server" -Database "DB" -Last

# Specific type (Full/Differential/Log)
Get-SqlDatabaseBackup -ServerInstance "Server" -Database "DB" -BackupActionType Full

# Output to file
Get-SqlDatabaseBackup -ServerInstance "Server" -Database "DB" -Path "C:\path\file.txt"
```
