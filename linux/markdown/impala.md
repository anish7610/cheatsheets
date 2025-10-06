# Impala Command in Linux

`impala` is a tool to interact with the Cloudera Impala service, a high-performance SQL engine for processing large volumes of data stored in Hadoop Distributed File System (HDFS).

## Common Options

| Option                   | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| `-i, --impalad=<host:port>` | Connect to a specific Impala daemon.                                       |
| `-d, --database=<database>` | Specify the database to use.                                               |
| `-q, --query=<query>`    | Execute a specific SQL query.                                                |
| `-f, --query_file=<file>`| Execute a query from a specified file.                                       |
| `-o, --output_file=<file>`| Write query results to a file.                                             |
| `-B`                     | Disable pretty printing for query results, useful for scripts.              |
| `-V, --verbose`          | Enable verbose output.                                                      |
| `-h, --help`             | Display help information.                                                   |

## Usage Examples

### Connect to an Impala Daemon
```bash
impala-shell -i impala-host:21000
```

### Execute a Query
```bash
impala-shell -i impala-host:21000 -q "SELECT * FROM my_table LIMIT 10;"
```

### Use a Specific Database
```bash
impala-shell -i impala-host:21000 -d my_database
```

### Execute a Query from a File
```bash
impala-shell -i impala-host:21000 -f query.sql
```

### Write Query Results to a File
```bash
impala-shell -i impala-host:21000 -q "SELECT * FROM my_table;" -o results.txt
```

### Disable Pretty Printing for Scripting
```bash
impala-shell -i impala-host:21000 -B -q "SELECT * FROM my_table LIMIT 10;"
```

## Cheat Sheet

```bash
# Connect
impala-shell -i <host:port>

# Query
impala-shell -q "<query>"

# File query
impala-shell -f <file>

# Output to file
impala-shell -o <output_file>

# Disable pretty
impala-shell -B
```

Replace `<host:port>`, `<query>`, `<file>`, and `<output_file>` with your specific values.
