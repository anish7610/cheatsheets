# Get-SqlServer Command

`Get-SqlServer` is a PowerShell command used to retrieve SQL Server instances and their properties. It is commonly used for database administration and management tasks.

## Common Options

| Option             | Description                                               |
|--------------------|-----------------------------------------------------------|
| `-ServerInstance`  | Specifies the SQL Server instance to connect to.          |
| `-Credential`      | Supplies a credential object for authentication.          |
| `-Namespace`       | Defines the SQL Server namespace (default: `root\Microsoft\SqlServer\ComputerManagement11`). |
| `-Verbose`         | Provides detailed information about the command's execution. |

## Usage Examples

### Example 1: Retrieve All SQL Server Instances

```powershell
Get-SqlServer
```

### Example 2: Retrieve a Specific SQL Server Instance

```powershell
Get-SqlServer -ServerInstance "MyServer\SQLInstance"
```

### Example 3: Use a Credential for Authentication

```powershell
$cred = Get-Credential
Get-SqlServer -ServerInstance "MyServer\SQLInstance" -Credential $cred
```

### Example 4: Verbose Output

```powershell
Get-SqlServer -Verbose
```

## Cheat Sheet

```plaintext
# Get all SQL Server instances
Get-SqlServer

# Get a specific instance
Get-SqlServer -ServerInstance "Server\Instance"

# Use specific credentials
$cred = Get-Credential
Get-SqlServer -ServerInstance "Server\Instance" -Credential $cred

# Enable verbose output
Get-SqlServer -Verbose
```
