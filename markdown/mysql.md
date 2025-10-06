# `mysql` Command Overview

The `mysql` command-line tool is used to interact with MySQL databases. It allows you to execute SQL queries, manage databases, and perform administrative tasks directly from the terminal.

## Common Options

| Option          | Description                                                                 |
|-----------------|-----------------------------------------------------------------------------|
| `-u, --user`    | Specify the MySQL username.                                                 |
| `-p, --password`| Prompt for the password.                                                    |
| `-h, --host`    | Connect to a different host.                                                |
| `-P, --port`    | Specify the port number for the connection.                                 |
| `-e, --execute` | Execute the given command and exit.                                         |
| `-D, --database`| Specify the default database to connect to.                                 |
| `--ssl`         | Enable SSL for the connection.                                              |
| `--skip-column-names` | Do not write column names in output.                                 |
| `-v, --verbose` | Enable verbose output.                                                      |

## Usage Examples

### Connecting to a Database

```bash
mysql -u username -p
```

This connects you to the MySQL server using the specified username. You'll be prompted for the password.

### Executing a Query

```bash
mysql -u username -p -e "SHOW DATABASES;"
```

Executes the query to list all databases and exits.

### Connecting to a Specific Host and Database

```bash
mysql -u username -p -h hostname -D database_name
```

Connects to a specified host and database.

### Exporting a Table to a File

```bash
mysql -u username -p -e "SELECT * FROM table_name;" database_name > output.txt
```

Exports the `table_name` contents to `output.txt`.

## Cheat Sheet

```plaintext
mysql -u [user] -p                      # Connect to MySQL server
mysql -u [user] -p -h [host]            # Connect to a specific host
mysql -u [user] -p -D [database]        # Select default database
mysql -u [user] -p -e "[query]"         # Execute query and exit
mysql -u [user] -p --ssl                # Connect using SSL
```
