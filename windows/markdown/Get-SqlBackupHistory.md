# `Get-SqlBackupHistory` Command Overview

`Get-SqlBackupHistory` is a Windows PowerShell command used to retrieve backup history information from SQL Server databases. It helps database administrators track and manage backup activities.

## Common Options

| Option                 | Description                                                  |
|------------------------|--------------------------------------------------------------|
| `-ServerInstance`      | Specifies the SQL Server instance to connect to.             |
| `-Database`            | Filters the results by the name of the database.             |
| `-StartDate`           | Filters backups starting from this date.                     |
| `-EndDate`             | Filters backups up to this date.                             |
| `-ResourceGroupName`   | Specifies the resource group (when used with Azure SQL).     |
| `-Credential`          | Provides the credentials for connecting to the SQL Server.   |

## Usage Examples

### Retrieve Backup History for a Specific Database

```powershell
Get-SqlBackupHistory -ServerInstance "MyServer" -Database "MyDatabase"
```

### Retrieve Backup History Within a Date Range

```powershell
Get-SqlBackupHistory -ServerInstance "MyServer" -StartDate "2023-01-01" -EndDate "2023-12-31"
```

### Retrieve Backup History Using Stored Credentials

```powershell
$cred = Get-Credential
Get-SqlBackupHistory -ServerInstance "MyServer" -Database "MyDatabase" -Credential $cred
```

## Cheat Sheet

```plaintext
# Basic structure
Get-SqlBackupHistory -ServerInstance "YourServer" -Database "YourDatabase"

# Date range filter
-StartDate "YYYY-MM-DD" -EndDate "YYYY-MM-DD"

# Using credentials
-Credential (Get-Credential)
```
