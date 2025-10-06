# Get-SqlDatabaseRestore Command

## Description

`Get-SqlDatabaseRestore` is a PowerShell command used to retrieve information about potential SQL Server database restores. It's commonly used by database administrators to check restore scenarios and plan restoration strategies.

## Common Options

| Option           | Description                                                  |
|------------------|--------------------------------------------------------------|
| `-ServerInstance`| Specifies the SQL Server instance to connect to.             |
| `-Database`      | Specifies the database to get restore information for.       |
| `-AsJob`         | Runs the command as a background job.                        |
| `-RestoreAction` | Defines the type of restore action (e.g., `Database`, `Log`).|
| `-Credential`    | Provides a credential object for SQL Server authentication.  |

## Usage Examples

### Example 1: Get Restore Information for a Specific Database
```powershell
Get-SqlDatabaseRestore -ServerInstance "localhost\SQLEXPRESS" -Database "SalesData"
```

### Example 2: Run the Restore Check as a Background Job
```powershell
Get-SqlDatabaseRestore -ServerInstance "localhost" -Database "HRData" -AsJob
```

### Example 3: Specify Credential for Server Authentication
```powershell
$cred = Get-Credential
Get-SqlDatabaseRestore -ServerInstance "RemoteServer" -Database "Finance" -Credential $cred
```

## Cheat Sheet

```plaintext
Get-SqlDatabaseRestore -ServerInstance "<server>" -Database "<db>"
```
