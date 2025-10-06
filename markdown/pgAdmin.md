# pgAdmin Command in Linux

`pgAdmin` is a popular open-source administration and management tool for PostgreSQL databases. It provides a graphical interface for database management, schema design, and data manipulation.

## Common Options

| Option         | Explanation                                              |
|----------------|----------------------------------------------------------|
| `--server`     | Specify server name/address to connect.                  |
| `--port`       | Define port number for connection (default: 5432).       |
| `--username`   | Set the user to connect as.                              |
| `--password`   | Provide password for the user.                           |
| `--dbname`     | Specify database name to connect to.                     |
| `--help`       | Display help information for the command.                |

## Usage Examples

### Connect to a PostgreSQL Database

To connect to a database on `localhost` with a specific user:

```shell
pgAdmin --server localhost --port 5432 --username admin --dbname mydb
```

### Troubleshooting Connection

To display help information if facing issues:

```shell
pgAdmin --help
```

## Quick Reference Cheat Sheet

```markdown
# pgAdmin Quick Reference

- Connect to a database:
  `pgAdmin --server [server] --port [port] --username [user] --dbname [db]`

- Display help:
  `pgAdmin --help`
```
