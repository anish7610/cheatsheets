# Hive Command in Linux

`hive` is a command-line interface for Apache Hive, a data warehouse software that facilitates reading, writing, and managing large datasets residing in distributed storage using SQL.

## Common Options

| Option                  | Description                                                  |
|-------------------------|--------------------------------------------------------------|
| `-e <query>`            | Execute the specified Hive query.                            |
| `-f <file>`             | Execute Hive queries in the file provided.                   |
| `-S`                    | Silent mode — only prints results, suppressing log details.  |
| `--database <database>` | Specify the database to use.                                 |
| `-i <init-file>`        | Initialization file with Hive commands to execute prior.     |

## Usage Examples

### Execute a Single Query

```bash
hive -e "SELECT * FROM employees WHERE salary > 50000;"
```

### Run Queries from a File

```bash
hive -f queries.sql
```

### Use a Specific Database

```bash
hive --database sales -e "SELECT * FROM transactions LIMIT 10;"
```

### Silent Mode for Clean Output

```bash
hive -S -e "SELECT COUNT(*) FROM orders;"
```

### Use an Initialization File

```bash
hive -i init.hql -e "SHOW TABLES;"
```

## Cheat Sheet

```plaintext
hive -e "query"                  # Execute a query
hive -f filename                 # Run queries from file
hive --database dbname -e "query" # Target specific database
hive -S -e "query"               # Silent mode (clean output)
hive -i initfile -e "query"      # Use initialization file
```
