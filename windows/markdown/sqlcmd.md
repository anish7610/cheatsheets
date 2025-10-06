## `sqlcmd` Command Overview

`sqlcmd` is a command-line utility used to interact with SQL Server from a Windows environment. It allows users to execute SQL queries, manage database objects, and perform various administrative tasks directly from the terminal.

## Common Options

| Option     | Description                                                   |
|------------|---------------------------------------------------------------|
| `-S`       | Specifies the SQL Server instance to connect to.              |
| `-U`       | Indicates the username for SQL Server authentication.         |
| `-P`       | Gives the password for the SQL Server account.                |
| `-d`       | Sets the default database for the connection.                 |
| `-Q`       | Executes a query directly and exits after completion.         |
| `-i`       | Specifies a script file to be executed.                       |
| `-o`       | Writes the output to a specified file.                        |
| `-E`       | Uses Windows Authentication for the connection.               |
| `-I`       | Sets the connection to be case insensitive.                   |

## Usage Examples

### Connecting to a Server and Running a Simple Query

```bash
sqlcmd -S myServer -U myUser -P myPassword -Q "SELECT name FROM master.sys.databases"
```

### Using Windows Authentication

```bash
sqlcmd -S myServer -E -Q "SELECT CURRENT_USER"
```

### Executing a Script File

```bash
sqlcmd -S myServer -U myUser -P myPassword -i myScript.sql
```

### Redirecting Output to a File

```bash
sqlcmd -S myServer -U myUser -P myPassword -Q "SELECT name FROM master.sys.databases" -o output.txt
```

## Cheat Sheet

```plaintext
# Connect and run a query
sqlcmd -S <server> -U <user> -P <password> -Q "<query>"

# Windows authentication
sqlcmd -S <server> -E -Q "<query>"

# Run a script from file
sqlcmd -S <server> -U <user> -P <password> -i <file.sql>

# Save output to file
sqlcmd -S <server> -U <user> -P <password> -Q "<query>" -o <output.txt>
```
