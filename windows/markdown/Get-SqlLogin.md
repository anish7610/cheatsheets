# Get-SqlLogin Command Overview

`Get-SqlLogin` is a PowerShell command used to retrieve SQL Server login information. It helps in managing security by listing logins and their properties on an SQL Server instance.

## Common Options

| Option           | Description                                                        |
|------------------|--------------------------------------------------------------------|
| `-ServerInstance`| Specifies the SQL Server instance to connect to.                   |
| `-Login`         | Filters so only the specified login is returned.                   |
| `-Credential`    | Specifies a user account to use for the connection.                |
| `-ErrorAction`   | Determines how the command handles non-terminating errors.         |

## Usage Examples

### Example 1: Retrieve All Logins
```powershell
Get-SqlLogin -ServerInstance "MyServerInstance"
```

### Example 2: Retrieve a Specific Login
```powershell
Get-SqlLogin -ServerInstance "MyServerInstance" -Login "UserLoginName"
```

### Example 3: Using Credentials for Connection
```powershell
$cred = Get-Credential
Get-SqlLogin -ServerInstance "MyServerInstance" -Credential $cred
```

## Cheat Sheet

```plaintext
# List all logins
Get-SqlLogin -ServerInstance "InstanceName"

# Filter by login name
Get-SqlLogin -ServerInstance "InstanceName" -Login "LoginName"

# Use specific credentials
$cred = Get-Credential
Get-SqlLogin -ServerInstance "InstanceName" -Credential $cred
```
