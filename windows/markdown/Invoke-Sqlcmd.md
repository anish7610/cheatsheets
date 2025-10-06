# Invoke-Sqlcmd Overview

`Invoke-Sqlcmd` is a PowerShell command used to run T-SQL commands or queries against a SQL Server database. It's part of the SQL Server module and is useful for automating database tasks and retrieving data.

## Common Options

| Option                   | Description                                                             |
|--------------------------|-------------------------------------------------------------------------|
| `-Query`                 | The T-SQL query to execute.                                             |
| `-QueryTimeout`          | Specifies how long to wait for the query to execute before timing out.  |
| `-ServerInstance`        | The SQL Server instance to connect to.                                  |
| `-Database`              | The target database to run the query against.                           |
| `-Username`              | The SQL Server username for authentication.                             |
| `-Password`              | The password for SQL Server authentication.                             |
| `-ConnectionTimeout`     | Time to wait for a connection before timing out.                        |
| `-OutputSqlErrors`       | Determines if errors from SQL Server are written to the console.        |
| `-Variable`              | Passes a T-SQL variable to the query.                                   |

## Usage Examples

### Example 1: Running a Simple Query

```powershell
Invoke-Sqlcmd -Query "SELECT * FROM Employees" -ServerInstance "localhost" -Database "HR"
```

### Example 2: Running a Query with Authentication

```powershell
Invoke-Sqlcmd -Query "SELECT * FROM Sales" -ServerInstance "localhost" -Database "SalesDB" -Username "admin" -Password "password123"
```

### Example 3: Using Variables in a Query

```powershell
Invoke-Sqlcmd -Query "SELECT * FROM Products WHERE CategoryID = $(CategoryID)" -ServerInstance "localhost" -Database "Store" -Variable @{ CategoryID = 5 }
```

## Cheat Sheet

```plaintext
Invoke-Sqlcmd -Query "<SQL_Query>" -ServerInstance "<Server>" -Database "<Database>"

# With SQL Auth
Invoke-Sqlcmd -Query "<SQL_Query>" -ServerInstance "<Server>" -Username "<Username>" -Password "<Password>"
```

Remember to replace placeholders with actual values pertinent to your SQL environment!
