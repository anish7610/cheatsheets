# `myloader` Command Overview

`myloader` is a part of the Mydumper suite, primarily used for parallel restoration of MySQL database backups. It is efficient for loading large datasets, making it ideal for scalable MySQL database management.

## Common Options

| Option                | Explanation                                           |
|-----------------------|-------------------------------------------------------|
| `-d, --directory`     | Directory containing the dumped files.                |
| `-h, --host`          | MySQL host to connect to.                             |
| `-u, --user`          | MySQL username.                                       |
| `-p, --password`      | MySQL password.                                       |
| `-P, --port`          | MySQL port number.                                    |
| `-t, --threads`       | Number of threads to use for restoring data.          |
| `-B, --database`      | Specify the database to restore.                      |
| `-o, --overwrite-tables` | Overwrite existing tables.                         |
| `-v, --verbose`       | Increase output verbosity.                            |

## Usage Examples

### Restore a Database with Multiple Threads
```bash
myloader -d /path/to/dump -u root -p yourpassword -t 4
```

### Restore a Specific Database
```bash
myloader -d /path/to/dump -u root -p yourpassword -B mydatabase
```

### Restore and Overwrite Existing Tables
```bash
myloader -d /path/to/dump -u root -p yourpassword -o
```

### Restore Data Hosted on a Specific Host and Port
```bash
myloader -d /path/to/dump -h dbhost.example.com -P 3307 -u root -p yourpassword
```

## Cheat Sheet

```plaintext
myloader -u [user] -p [password] -d [directory] [options]

-d  Specify dump directory
-t  Set number of threads
-B  Specify database
-o  Overwrite existing tables

# Basic example
myloader -d /dump -u root -p pass
```

> Adjust thread and host options according to server capabilities and configuration.
