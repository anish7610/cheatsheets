# `netstat` Command in Linux

## Description

`netstat` (network statistics) is a command-line utility that provides network-related information such as active connections, routing tables, interface statistics, masquerade connections, and multicast memberships.

## Common Options

| Option | Description                                      |
|--------|--------------------------------------------------|
| `-a`   | Show all sockets (including listening).          |
| `-t`   | Display TCP connections.                         |
| `-u`   | Display UDP connections.                         |
| `-l`   | Show only listening ports.                       |
| `-n`   | Show numerical addresses instead of resolving.   |
| `-p`   | Show the PID and name of the program using the socket. |
| `-r`   | Display the routing table.                       |
| `-s`   | Display network statistics.                      |
| `-i`   | Display network interfaces.                      |

## Usage Examples

### List All Network Connections
```bash
netstat -a
```

### Display TCP Connections
```bash
netstat -t
```

### Show Listening Ports
```bash
netstat -l
```

### Display Numerical Addresses
```bash
netstat -n
```

### Show Active Connections with Program Names
```bash
sudo netstat -p
```

### View the Routing Table
```bash
netstat -r
```

### Display Network Statistics
```bash
netstat -s
```

## Cheat Sheet

```bash
netstat -an       # Show all connections numerically
netstat -tuln     # Show listening TCP/UDP ports
netstat -i        # Display network interfaces
netstat -rn       # Display routing table numerically
```
