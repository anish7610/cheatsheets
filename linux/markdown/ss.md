# `ss` Command in Linux

## Description

The `ss` command in Linux is used to display network socket information. It's a modern replacement for the older `netstat` command, providing more detailed information efficiently about network connections, sockets, and listening ports.

## Common Options

| Option | Description                                 |
|--------|---------------------------------------------|
| `-t`   | Display TCP sockets.                        |
| `-u`   | Display UDP sockets.                        |
| `-l`   | Show listening sockets.                     |
| `-p`   | Show process using the socket.              |
| `-n`   | Display numerical addresses instead of resolving hostnames. |
| `-a`   | Display all sockets (listening and non-listening). |
| `-4`   | Display only IPv4 sockets.                  |
| `-6`   | Display only IPv6 sockets.                  |
| `-s`   | Display summary statistics.                 |

## Usage Examples

### Display All Listening TCP Sockets

```bash
ss -tl
```

### Show All UDP Sockets

```bash
ss -au
```

### Display Sockets with Listening State, Numerical Addresses, and Processes

```bash
ss -ltnp
```

### Show IPv4 Sockets

```bash
ss -4
```

### View Summary Statistics

```bash
ss -s
```

## Cheat Sheet

```
ss -tl     # List TCP listening sockets
ss -au     # List all UDP sockets
ss -ltnp   # List listening sockets with process info
ss -4      # List IPv4 sockets
ss -s      # Display socket summary
```
