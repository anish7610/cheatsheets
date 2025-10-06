# PostgreSQL Command

The `postgresql` command typically refers to interacting with PostgreSQL databases through various command-line tools like `psql`, `pg_ctl`, etc. These tools are used to manage, query, and control PostgreSQL databases.

## Common Options

| Option          | Description                                          |
|-----------------|------------------------------------------------------|
| `-h`            | Specify the host of the database server.             |
| `-p`            | Specify the port on which the database server is listening. |
| `-U`            | Specify the username to connect as.                  |
| `-d`            | Specify the name of the database to connect to.      |
| `-f`            | Execute commands from a file.                        |
| `-c`            | Execute a single command and exit.                   |
| `-l`            | List available databases.                            |

## Usage Examples

### Connect to a Database

```bash
psql -h localhost -p 5432 -U username -d database_name
```

### Execute SQL from a File

```bash
psql -U username -d database_name -f script.sql
```

### Execute a Single Command

```bash
psql -U username -d database_name -c "SELECT * FROM table_name;"
```

### List Databases

```bash
psql -U username -l
```

## Cheat Sheet

```plaintext
psql -h host -p port -U user -d db                # Connect to database
psql -U user -d db -f file.sql                    # Execute SQL file
psql -U user -d db -c "SQL Command"               # Run single command
```
