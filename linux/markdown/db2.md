# `db2` Command Overview

The `db2` command interfaces with IBM Db2 databases, providing tools for SQL querying, database management, and script execution. It's widely used for database administration and application development tasks.

## Common Options

| Option          | Explanation                                    |
|-----------------|------------------------------------------------|
| `-td` `<char>`  | Sets the statement termination character.      |
| `-f` `<file>`   | Specifies a script file to be executed.        |
| `-r` `<file>`   | Redirects command output to a specified file.  |
| `-z` `<file>`   | Redirects messages to a specified file.        |
| `+c`            | Continues on errors without stopping execution.|

## Usage Examples

### Execute a SQL Script

```bash
db2 -td ";" -f myscript.sql
```

*Executes SQL commands in `myscript.sql`, using `;` as the statement terminator.*

### Redirect Output and Errors

```bash
db2 -f myscript.sql -r output.txt -z errors.txt
```

*Executes `myscript.sql`, redirecting output to `output.txt` and errors to `errors.txt`.*

### Execute Inline SQL Command

```bash
db2 "SELECT * FROM users"
```

*Executes a direct SQL query on the `users` table.*

### Continue on Errors

```bash
db2 +c -f myscript.sql
```

*Executes `myscript.sql`, continuing past errors.*

## Cheat Sheet

```plaintext
Execute SQL Script: db2 -td ";" -f script.sql
Redirect Output: db2 -f script.sql -r output.txt
Inline SQL Command: db2 "SELECT * FROM table"
Continue on Errors: db2 +c -f script.sql
```

Use this guide as a quick reference for common `db2` command tasks. Adjust parameters as needed to fit specific use cases.
