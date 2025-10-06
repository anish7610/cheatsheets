# Get-SqlTable Command Overview

`Get-SqlTable` is a PowerShell command used to retrieve information about tables from a specified SQL Server database.

## Common Options

| Option           | Description                                               |
|------------------|-----------------------------------------------------------|
| `-ServerInstance`| Specifies the name of the SQL Server instance.            |
| `-Database`      | Specifies the name of the database to query.              |
| `-Schema`        | Filters tables by schema name.                            |
| `-TableName`     | Filters by specific table name. Supports wildcards.       |
| `-Credential`    | Specifies a user account to use for the connection.       |
| `-OutputAs`      | Determines the format of the output (`DataTable`, `PSObject`). |

## Usage Examples

### Example 1: List All Tables in a Database

```powershell
Get-SqlTable -ServerInstance "localhost" -Database "AdventureWorks"
```

### Example 2: List Tables in a Specific Schema

```powershell
Get-SqlTable -ServerInstance "localhost" -Database "AdventureWorks" -Schema "Sales"
```

### Example 3: Find a Specific Table Using Wildcards

```powershell
Get-SqlTable -ServerInstance "localhost" -Database "AdventureWorks" -TableName "Emp*"
```

### Example 4: Use Credentials for Connection

```powershell
$credential = Get-Credential
Get-SqlTable -ServerInstance "localhost" -Database "AdventureWorks" -Credential $credential
```

## Cheat Sheet

```plaintext
# Basic Usage
Get-SqlTable -ServerInstance "server" -Database "db"

# Filter by Schema
Get-SqlTable -Schema "schema"

# Filter by Table Name
Get-SqlTable -TableName "name"

# Use Credentials
$cred = Get-Credential
Get-SqlTable -Credential $cred
```
