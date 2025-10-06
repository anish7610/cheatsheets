# Remove-SqlDatabase Command

`Remove-SqlDatabase` is a PowerShell command used to delete a database from a SQL Server instance.

## Common Options

| Option                 | Explanation                                                      |
|------------------------|------------------------------------------------------------------|
| `-ServerInstance`      | Specifies the SQL Server instance name.                          |
| `-Database`            | Names the database to be removed.                                |
| `-Force`               | Removes the database without prompting for confirmation.         |
| `-Confirm`             | Prompts for confirmation before executing the removal.           |
| `-Credential`          | Specifies a user credential for authentication on the server.    |

## Usage Examples

### Example 1: Remove a Database with Confirmation
```powershell
Remove-SqlDatabase -ServerInstance "MyServer" -Database "TestDatabase" -Confirm
```

### Example 2: Forcefully Remove a Database Without Confirmation
```powershell
Remove-SqlDatabase -ServerInstance "MyServer" -Database "TestDatabase" -Force
```

### Example 3: Remove a Database Using Credentials
```powershell
$cred = Get-Credential
Remove-SqlDatabase -ServerInstance "MyServer" -Database "TestDatabase" -Credential $cred
```

## Cheat Sheet

```plaintext
Remove-SqlDatabase -ServerInstance <Server> -Database <Database> [-Force] [-Credential <Credentials>] [-Confirm]
```

Replace `<Server>` and `<Database>` with your specific server name and database name.
