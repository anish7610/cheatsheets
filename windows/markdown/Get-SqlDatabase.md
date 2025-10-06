# Get-SqlDatabase Command in PowerShell

## Description

`Get-SqlDatabase` is a PowerShell command used to retrieve information about databases on an instance of SQL Server. It's part of the SQL Server module, allowing users to query database properties and perform administrative tasks.

## Common Options

| Option                      | Description                                                     |
|-----------------------------|-----------------------------------------------------------------|
| `-ServerInstance`           | Specifies the SQL Server instance to query.                     |
| `-Database`                 | Filters the results by a specific database name.                |
| `-Credential`               | Specifies a user credential for authentication.                 |
| `-InformationAction`        | Specifies how to respond to an information event.               |
| `-InformationVariable`      | Specifies a variable to store information event messages.       |

## Usage Examples

### List All Databases on a Server

```powershell
Get-SqlDatabase -ServerInstance "MyServer\SQLInstance"
```

### Get a Specific Database

```powershell
Get-SqlDatabase -ServerInstance "MyServer\SQLInstance" -Database "MyDatabase"
```

### Using Credentials

```powershell
$cred = Get-Credential
Get-SqlDatabase -ServerInstance "MyServer\SQLInstance" -Credential $cred
```

## Cheat Sheet

```plaintext
List databases:
  Get-SqlDatabase -ServerInstance "Server\Instance"

Get specific database:
  Get-SqlDatabase -ServerInstance "Server\Instance" -Database "DBName"

Use credentials:
  $cred = Get-Credential
  Get-SqlDatabase -ServerInstance "Server\Instance" -Credential $cred
```
