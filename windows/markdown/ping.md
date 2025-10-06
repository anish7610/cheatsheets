# `ping` Command Overview

The `ping` command is used to test the reachability of a host on an IP network and to measure the round-trip time for messages sent from the originating host to a destination computer.

## Common Options

| Option         | Description                                         |
|----------------|-----------------------------------------------------|
| `-t`           | Ping the specified host until stopped.              |
| `-n count`     | Number of echo requests to send.                    |
| `-l size`      | Send buffer size.                                   |
| `-4`           | Force using IPv4.                                   |
| `-6`           | Force using IPv6.                                   |
| `-w timeout`   | Timeout in milliseconds to wait for each reply.     |

## Usage Examples

### Ping a Host Continuously
```bash
ping -t example.com
```

### Send a Specific Number of Pings
```bash
ping -n 5 example.com
```

### Specify Buffer Size
```bash
ping -l 1024 example.com
```

### Force IPv4
```bash
ping -4 example.com
```

### Force IPv6
```bash
ping -6 example.com
```

### Set Timeout
```bash
ping -w 1000 example.com
```

## Cheat Sheet

```plaintext
ping -t <host>         # Ping until stopped
ping -n <count> <host> # Send specific number of packets
ping -l <size> <host>  # Define buffer size
ping -4 <host>         # Force IPv4
ping -6 <host>         # Force IPv6
ping -w <ms> <host>    # Set timeout in milliseconds
```
