# `cassandra` Command in Linux

## Description
The `cassandra` command is used to start the Apache Cassandra database server, which is a highly scalable, distributed NoSQL database designed to handle large amounts of data across many commodity servers with no single point of failure.

## Common Options

| Option              | Description                                        |
|---------------------|----------------------------------------------------|
| `-f, --foreground`  | Run Cassandra in the foreground. Useful for debugging. |
| `-p <pidfile>`      | Write the process ID of the server to the specified file. |
| `-R, --ring-delay`  | Set the delay (in milliseconds) before joining the ring. |
| `-Dcassandra.config`| Specify an alternative configuration file.         |

## Usage Examples

### Start Cassandra in Foreground

```bash
cassandra -f
```

### Specify a Custom Configuration File

```bash
cassandra -Dcassandra.config=/path/to/custom.yaml
```

### Write Process ID to a File

```bash
cassandra -p /var/run/cassandra.pid
```

### Set Delay Before Joining the Ring

```bash
cassandra -R 5000
```

## Cheat Sheet

```markdown
# Start Cassandra in the foreground
cassandra -f

# Use custom configuration
cassandra -Dcassandra.config=/path/to/config.yaml

# Write PID to file
cassandra -p /path/to/pidfile

# Set ring join delay
cassandra -R <milliseconds>
```

Use this cheat sheet as a quick reference for starting and configuring the Apache Cassandra server using the `cassandra` command.
