# New-SqlDatabase Command

`New-SqlDatabase` is a PowerShell command used to create a new SQL Server database. It is part of the `SqlServer` module and allows users to define properties for the new database.

## Common Options

| Option             | Description                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| `-Name`            | Specifies the name of the new database.                                     |
| `-ServerInstance`  | Defines the SQL Server instance to connect to.                              |
| `-Collation`       | Sets the collation for the database.                                        |
| `-MaxSize`         | Specifies the maximum size of the database in megabytes.                    |
| `-DataFileSize`    | Sets the initial size of the database data file.                            |
| `-LogFileSize`     | Sets the initial size of the database log file.                             |
| `-PrimaryFilePath` | Sets the file path for the primary data file (*.mdf).                       |
| `-LogFilePath`     | Sets the file path for the log file (*.ldf).                                |

## Usage Examples

### Create a Simple Database

```powershell
New-SqlDatabase -Name "MyDatabase" -ServerInstance "localhost"
```

### Create a Database with Specific Size and Collation

```powershell
New-SqlDatabase -Name "MyDatabase" -ServerInstance "localhost" -Collation "SQL_Latin1_General_CP1_CI_AS" -DataFileSize 100MB -LogFileSize 50MB
```

### Create a Database with Max Size and Specific File Paths

```powershell
New-SqlDatabase -Name "MyDatabase" -ServerInstance "localhost" -MaxSize 500MB -PrimaryFilePath "C:\SQLData\MyDatabase.mdf" -LogFilePath "C:\SQLLogs\MyDatabase.ldf"
```

## Cheat Sheet

```plaintext
New-SqlDatabase -Name <DBName> -ServerInstance <Server> [-Collation <Collation>] [-MaxSize <SizeMB>]
```
