# `sqlite3` Command

`sqlite3` is a command-line interface for interacting with SQLite databases. It allows for executing SQL commands, managing tables, and performing queries directly from the terminal.

## Common Options

| Option       | Description                                                 |
|--------------|-------------------------------------------------------------|
| `.open`      | Opens an SQLite database file.                              |
| `.backup`    | Creates a backup of the database to a specified file.       |
| `.restore`   | Restores the database from a backup file.                   |
| `.tables`    | Lists all tables in the database.                           |
| `.schema`    | Shows the SQL schema of tables or a specific table.         |
| `.exit`      | Exits the SQLite shell.                                     |
| `.import`    | Imports data from a CSV file into a table.                  |
| `.mode`      | Sets output mode (e.g., `csv`, `column`, `list`).           |
| `.headers`   | Toggles display of column headers in the output.            |
| `.help`      | Displays help text for available commands.                  |

## Usage Examples

### Open a Database

```shell
sqlite3 my_database.db
```

### List All Tables

```shell
sqlite3 my_database.db ".tables"
```

### Show Schema of a Specific Table

```shell
sqlite3 my_database.db ".schema my_table"
```

### Import Data from CSV

```shell
sqlite3 my_database.db ".mode csv"
sqlite3 my_database.db ".import data.csv my_table"
```

### Backup a Database

```shell
sqlite3 my_database.db ".backup backup.db"
```

### Execute SQL Query

```shell
sqlite3 my_database.db "SELECT * FROM my_table WHERE column = 'value';"
```

## Cheat Sheet

```plaintext
Open:       sqlite3 my_database.db
List Tables:.tables
Show Schema:.schema [table]
Backup:     .backup backup.db
Import CSV: .mode csv
            .import file.csv table
Query:      "SELECT * FROM table;"
Exit:       .exit
```
