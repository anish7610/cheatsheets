# `cqlsh` Command Overview

`cqlsh` is a command-line shell for interacting with Apache Cassandra. It allows you to execute Cassandra Query Language (CQL) commands, manage clusters, and perform data operations.

## Common Options

| Option                       | Description                                      |
|------------------------------|--------------------------------------------------|
| `-u, --username`             | Specify the Cassandra username.                  |
| `-p, --password`             | Specify the Cassandra password.                  |
| `-f, --file`                 | Execute commands from a CQL file.                |
| `-k, --keyspace`             | Set the default keyspace.                        |
| `-e, --execute`              | Execute a single CQL command and exit.           |
| `--cqlversion`               | Specify the CQL version to be used.              |
| `--ssl`                      | Enable SSL for connecting to the database.       |
| `--debug`                    | Enable detailed debug output.                    |
| `--encoding`                 | Specify the text encoding used by the session.   |
| `-h, --host`                 | Specify the host to connect to.                  |
| `-p, --port`                 | Specify the port to use.                         |

## Usage Examples

### Connect to a Cassandra Cluster

```bash
cqlsh -u username -p password -h cassandra_host -p 9042
```

### Execute a CQL Script from a File

```bash
cqlsh -f script.cql
```

### Execute a Single CQL Command

```bash
cqlsh -e "SELECT * FROM keyspace_name.table_name LIMIT 10;" -u username -p password -h cassandra_host
```

### Use a Specific Keyspace

```bash
cqlsh -k keyspace_name
```

### Enable SSL Connection

```bash
cqlsh --ssl -u username -p password -h cassandra_host
```

## Cheat Sheet

```plaintext
Connect: cqlsh -u <user> -p <pass> -h <host> -p <port>
Execute CQL File: cqlsh -f <file>
Execute Command: cqlsh -e "<CQL>" -u <user> -p <pass>
Use Keyspace: cqlsh -k <keyspace>
Enable SSL: cqlsh --ssl
```
