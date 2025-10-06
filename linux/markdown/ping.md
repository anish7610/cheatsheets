# `ping` Command

The `ping` command is used to test the reachability of a host on a network. It works by sending Internet Control Message Protocol (ICMP) Echo Request packets to the target host and listening for Echo Reply packets.

## Common Options

| Option     | Description                                      |
|------------|--------------------------------------------------|
| `-c`       | Specify the number of packets to send.           |
| `-i`       | Set the interval in seconds between packets.     |
| `-t`       | Set the Time to Live (TTL) for packets.          |
| `-q`       | Quiet output. Only summary at the end.           |
| `-s`       | Specify the number of data bytes to be sent.     |
| `-W`       | Set the timeout in seconds to wait for a reply.  |
| `-f`       | Flood ping. Sends packets as fast as possible.   |

## Usage Examples

### Basic Ping
Test connectivity to `google.com` by sending the default number of packets:
```bash
ping google.com
```

### Specify Packet Count
Send exactly 5 packets to `example.com`:
```bash
ping -c 5 example.com
```

### Set Interval Between Pings
Send a packet every 2 seconds:
```bash
ping -i 2 example.com
```

### Quiet Mode
Only output a summary after 5 pings:
```bash
ping -c 5 -q example.com
```

### Specify Packet Size
Send packets with 64 bytes of data:
```bash
ping -s 64 example.com
```

## Cheat Sheet

```plaintext
ping [host]                     # Basic ping
ping -c [count] [host]          # Ping with count
ping -i [interval] [host]       # Ping with interval
ping -q -c [count] [host]       # Quiet ping with count
ping -s [size] [host]           # Ping with packet size
```
