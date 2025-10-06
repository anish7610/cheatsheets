# `mongosh` Command

`mongosh` is the MongoDB Shell, an interactive JavaScript interface for MongoDB. It allows you to connect to a MongoDB server, execute database operations, and manage your database.

## Common Options

| Option                     | Description                                      |
|----------------------------|--------------------------------------------------|
| `--host <hostname>`        | Specify the MongoDB server hostname.             |
| `--port <port>`            | Specify the MongoDB server port. (Default is 27017) |
| `--username <username>`    | Username for authentication.                     |
| `--password <password>`    | Password for authentication.                     |
| `--authenticationDatabase <db>` | Database to authenticate against.            |
| `--tls`                    | Enable connection via TLS/SSL.                   |
| `--quiet`                  | Suppress output for interactive use.             |

## Usage Examples

### Connect to a Local MongoDB Instance
```bash
mongosh
```

### Connect to a Remote MongoDB Instance
```bash
mongosh --host example.com --port 27018
```

### Connect with Authentication
```bash
mongosh --username admin --password secret --authenticationDatabase admin
```

### Connect Using TLS
```bash
mongosh --host example.com --tls
```

## Cheat Sheet

```bash
# Start shell with default connection
mongosh

# Connect to a specific host and port
mongosh --host <hostname> --port <port>

# Connect with authentication
mongosh --username <user> --password <pass> --authenticationDatabase <db>

# Connect using TLS
mongosh --host <hostname> --tls
```
