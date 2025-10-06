# `redis-cli` Command

`redis-cli` is a command-line interface tool used to interact with a Redis server. It allows you to execute Redis commands, test scripts, and manage your data.

## Common Options

| Option           | Explanation                                     |
|------------------|-------------------------------------------------|
| `-h <hostname>`  | Specify the Redis server hostname (default: 127.0.0.1). |
| `-p <port>`      | Specify the Redis server port (default: 6379).        |
| `-a <password>`  | Provide a password to authenticate with the server.    |
| `--stat`         | Display real-time server statistics.                   |
| `--scan`         | Iteratively scan the keys space.                      |
| `--rdb <file>`   | Export the database to an RDB file.                    |

## Usage Examples

### Connect to a Redis Server
```bash
redis-cli -h localhost -p 6379
```

### Authenticate with a Password
```bash
redis-cli -a yourpassword
```

### Display Server Statistics
```bash
redis-cli --stat
```

### Retrieve a Value by Key
```bash
redis-cli GET mykey
```

### Set a Key-Value Pair
```bash
redis-cli SET mykey "Hello, World!"
```

### Scan Keys
```bash
redis-cli --scan
```

### Backup the Database
```bash
redis-cli --rdb dump.rdb
```

## Cheat Sheet

```markdown
# Connect and authenticate
redis-cli -h <host> -p <port> -a <password>

# Get/Set keys
redis-cli GET <key>
redis-cli SET <key> <value>

# Display stats and scan
redis-cli --stat
redis-cli --scan

# Export database
redis-cli --rdb <file>
```
