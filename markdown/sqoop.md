# Linux `sqoop` Command

Sqoop is a tool designed to transfer data between Hadoop and relational database servers. It is used to import data from external datastores into Hadoop Distributed File System (HDFS) or export data from Hadoop to external databases.

## Common Options

| Option                | Description                                                                 |
|-----------------------|-----------------------------------------------------------------------------|
| `--connect`           | Connection JDBC URL to the database.                                        |
| `--username`          | Database username.                                                          |
| `--password`          | Database password.                                                          |
| `--table`             | Table to import or export.                                                  |
| `--target-dir`        | HDFS destination directory for import.                                      |
| `--export-dir`        | Source directory for export, in HDFS.                                       |
| `--num-mappers`       | Number of map tasks. More tasks increase parallelism.                       |
| `--incremental`       | Perform an incremental import. Options: `append`, `lastmodified`.           |
| `--check-column`      | Column to check for incremental import.                                     |
| `--last-value`        | Last value to use for an incremental import.                                |
| `--fields-terminated-by` | Specifies the field delimiter for imported data.                         |

## Usage Examples

### Import a Table from MySQL to HDFS

```bash
sqoop import \
  --connect jdbc:mysql://localhost/database_name \
  --username user \
  --password pass \
  --table table_name \
  --mappers 4 \
  --target-dir /user/hadoop/data
```

### Export Data from HDFS to MySQL

```bash
sqoop export \
  --connect jdbc:mysql://localhost/database_name \
  --username user \
  --password pass \
  --table table_name \
  --export-dir /user/hadoop/data \
  --mappers 4
```

### Incremental Import

```bash
sqoop import \
  --connect jdbc:mysql://localhost/database_name \
  --username user \
  --password pass \
  --table table_name \
  --incremental append \
  --check-column id \
  --last-value 100 \
  --target-dir /user/hadoop/data
```

## Cheat Sheet

```plaintext
# Import table
sqoop import --connect jdbc:[connection] --username [user] --password [pass] --table [table] --target-dir [dir]

# Export table
sqoop export --connect jdbc:[connection] --username [user] --password [pass] --table [table] --export-dir [dir]

# Incremental import
sqoop import --connect jdbc:[connection] --username [user] --password [pass] --table [table] --incremental [mode] --check-column [column] --last-value [value] --target-dir [dir]
```

Use Sqoop to efficiently transfer large amounts of data between Hadoop and relational database systems, leveraging its parallel processing capabilities with customized options.
