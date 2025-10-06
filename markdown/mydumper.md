# mydumper Command Overview

`mydumper` is a high-performance tool for MySQL database backups. It provides parallel processing, making the backup process faster compared to traditional methods.

## Common Options

| Option                 | Description                                                            |
|------------------------|------------------------------------------------------------------------|
| `-B, --database`       | Specify a specific database to dump.                                   |
| `-T, --tables-list`    | List of specific tables to dump (format: db.table).                    |
| `-o, --outputdir`      | Directory to store the output files.                                   |
| `-r, --rows`           | Split tables into chunks of `rows` rows.                               |
| `--build-empty-files`  | Create empty files if no data is available for specified tables.       |
| `-e, --exec`           | Execute extra commands after dump (useful for flushing caches).        |
| `-p, --password`       | Password to connect to the database.                                   |
| `-u, --user`           | Username to connect to the database.                                   |
| `-h, --host`           | MySQL host to connect to (default is 'localhost').                     |
| `-P, --port`           | MySQL port to connect to (default is 3306).                            |
| `-c, --compress`       | Compress the output files using gzip.                                  |
| `-v, --verbose`        | Increase verbosity, helpful for debugging.                             |

## Usage Examples

### Backup a Specific Database
```bash
mydumper -u root -p password -h localhost -P 3306 -B mydatabase -o /backup/mydatabase
```

### Backup with Specified Tables
```bash
mydumper -u root -p password -B mydatabase -T mytable1,mytable2 -o /backup/specific_tables
```

### Backup and Compress the Output
```bash
mydumper -u root -p password -B mydatabase -o /backup/compressed_backup -c
```

### Split Tables into Chunks of 1000 Rows
```bash
mydumper -u root -p password -B mydatabase -o /backup/chunks -r 1000
```

## Cheat Sheet

```
# Backup entire database
mydumper -u <user> -p <password> -B <database> -o <outputdir>

# Backup specific tables
mydumper -u <user> -p <password> -B <database> -T <table1,table2> -o <outputdir>

# Compress output
mydumper -u <user> -p <password> -B <database> -o <outputdir> -c
```
