# Get-SqlUser Command

`Get-SqlUser` is a PowerShell command used to retrieve SQL Server database user information.

## Common Options

| Option              | Explanation                                              |
|---------------------|----------------------------------------------------------|
| `-ServerInstance`   | Specifies the SQL Server instance name.                  |
| `-Database`         | Specifies the database to query for users.               |
| `-Username`         | Filters results by a specific username.                  |
| `-Credential`       | Provides user credentials for authentication.            |
| `-DisableException` | Continues processing on errors, suppressing exceptions.  |

## Usage Examples

### Example 1: Retrieve all users from a specified database
```powershell
Get-SqlUser -ServerInstance "MyServer\SQLInstance" -Database "MyDB"
```

### Example 2: Retrieve a specific user
```powershell
Get-SqlUser -ServerInstance "MyServer\SQLInstance" -Database "MyDB" -Username "jdoe"
```

### Example 3: Use credentials to retrieve users
```powershell
$cred = Get-Credential
Get-SqlUser -ServerInstance "MyServer\SQLInstance" -Database "MyDB" -Credential $cred
```

## Cheat Sheet

```plaintext
# Retrieve all users
Get-SqlUser -ServerInstance "Server" -Database "DB"

# Retrieve specific user
Get-SqlUser -ServerInstance "Server" -Database "DB" -Username "user"

# Using credentials
$cred = Get-Credential
Get-SqlUser -ServerInstance "Server" -Database "DB" -Credential $cred
```
