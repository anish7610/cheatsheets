## `mongod` Command

### Description

`mongod` is the primary daemon process for MongoDB. It handles data requests, manages data access, and performs background management operations.

### Common Options

| Option                   | Description                                                        |
|--------------------------|--------------------------------------------------------------------|
| `--port <number>`        | Specifies the port for incoming connections (default: 27017).      |
| `--dbpath <path>`        | File path where the database files are stored.                     |
| `--logpath <path>`       | File path to log MongoDB operations.                               |
| `--bind_ip <IP address>` | Comma-separated list of IP addresses to listen on (default: localhost). |
| `--fork`                 | Run `mongod` as a daemon in the background.                        |
| `--auth`                 | Enable authentication, requiring login for access.                 |
| `--config <path>`        | Path to a configuration file.                                      |

### Usage Examples

Start `mongod` with default settings:

```bash
mongod
```

Start `mongod` on a specific port and use a different database path:

```bash
mongod --port 27018 --dbpath /data/db2
```

Run `mongod` as a daemon, logging to a specific file:

```bash
mongod --fork --logpath /var/log/mongodb/mongod.log
```

Bind `mongod` to a specific IP address:

```bash
mongod --bind_ip 192.168.1.100
```

Enable authentication:

```bash
mongod --auth
```

Start `mongod` using a configuration file:

```bash
mongod --config /etc/mongod.conf
```

### Cheat Sheet

```plaintext
# Start with default
mongod

# Custom port and dbpath
mongod --port <number> --dbpath <path>

# Daemonize with logging
mongod --fork --logpath <path>

# Bind to IP
mongod --bind_ip <IP address>

# Enable authentication
mongod --auth

# Use configuration file
mongod --config <path>
```
