# `psql` Command Overview

`psql` is a command-line client for interacting with PostgreSQL databases. It allows users to execute SQL queries, manage database objects, and administer databases.

## Common Options

| Option | Description                                      |
|--------|--------------------------------------------------|
| `-h`   | Specify the host of the database server.         |
| `-p`   | Specify the port of the database server.         |
| `-U`   | Specify the database user name.                  |
| `-d`   | Specify the database name to connect to.         |
| `-c`   | Execute a single SQL command and exit.           |
| `-f`   | Execute commands from a file.                    |
| `-l`   | List all databases on the server.                |
| `-W`   | Prompt for the password before connecting.       |

## Usage Examples

### Connect to a Database

```bash
psql -h localhost -U username -d mydatabase
```

### Execute a Single SQL Command

```bash
psql -U username -d mydatabase -c "SELECT * FROM my_table;"
```

### Execute Commands from a File

```bash
psql -U username -d mydatabase -f /path/to/sqlfile.sql
```

### List All Databases

```bash
psql -l
```

### Prompt for Password

```bash
psql -h localhost -U username -W -d mydatabase
```

## Cheat Sheet

```plaintext
psql -h <host> -U <user> -d <dbname>     # Connect to database
psql -c "<SQL command>"                  # Execute SQL command
psql -f <file.sql>                       # Execute SQL file
psql -l                                  # List databases
psql -W                                  # Prompt for password
```
