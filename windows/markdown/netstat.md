# `netstat` Command in Windows

`netstat` is a command-line utility that displays network connections, routing tables, interface statistics, and more. It's useful for monitoring and troubleshooting network issues.

## Common Options

| Option        | Description                                                                           |
|---------------|---------------------------------------------------------------------------------------|
| `-a`          | Displays all connections and listening ports.                                         |
| `-n`          | Displays addresses and port numbers in numerical form.                                |
| `-b`          | Shows the executable involved in creating each connection or listening port. Requires elevated command prompt. |
| `-e`          | Displays Ethernet statistics, such as the number of bytes and packets sent and received. |
| `-o`          | Displays the owning process ID for each connection.                                   |
| `-p <proto>`  | Shows connections for the specified protocol (`TCP` or `UDP`).                        |
| `-r`          | Displays the routing table.                                                           |
| `-s`          | Displays statistics by protocol.                                                      |
| `-t`          | Displays the current connection offload state.                                        |

## Usage Examples

### Listing All Connections and Listening Ports
```shell
netstat -a
```

### Showing Connections with Process ID
```shell
netstat -o
```

### Displaying Address and Port Numbers Numerically
```shell
netstat -n
```

### Displaying Routing Table
```shell
netstat -r
```

### Viewing Statistics by Protocol
```shell
netstat -s
```

### Showing Executables Involved in Each Connection
```shell
netstat -b
```

## Cheat Sheet

```plaintext
netstat -a  # All connections and listening ports
netstat -n  # Numerical addresses and ports
netstat -b  # Executables (requires admin)
netstat -o  # Connections with process ID
netstat -r  # Routing table
netstat -s  # Protocol statistics
```
