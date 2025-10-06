# `tcpdump` Command

`tcpdump` is a powerful command-line packet analyzer tool used to capture, display, and analyze network traffic passing through a network interface.

## Common Options

| Option               | Description                                               |
|----------------------|-----------------------------------------------------------|
| `-i <interface>`     | Specify the network interface to listen on.               |
| `-nn`                | Display numeric addresses rather than resolving hostnames or port names. |
| `-X`                 | Show packet contents in both hex and ASCII.               |
| `-w <file>`          | Write captured packets to a file for later analysis.      |
| `-r <file>`          | Read packets from a saved file.                           |
| `-c <count>`         | Capture only a specified number of packets.               |
| `-v`, `-vv`, `-vvv`  | Increase the verbosity of output.                         |
| `-s <snaplen>`       | Define the snapshot length. Default is usually 65535.     |
| `-e`                 | Display link-layer header information.                    |
| `-A`                 | Display packets in ASCII.                                 |

## Usage Examples

### Capture Packets on a Specific Interface
```bash
tcpdump -i eth0
```

### Capture a Specific Number of Packets
```bash
tcpdump -c 10
```

### Capture Packets and Save to a File
```bash
tcpdump -i eth0 -w capture.pcap
```

### Read Packets from a File
```bash
tcpdump -r capture.pcap
```

### Capture Packets Without Resolving Hostnames
```bash
tcpdump -i eth0 -nn
```

### Display Content in Hex and ASCII
```bash
tcpdump -X -c 5
```

## Cheat Sheet

```plaintext
tcpdump -i <interface>    # Capture traffic on an interface
tcpdump -nn -X            # Numeric output; hex and ASCII display
tcpdump -w <file>         # Write packets to file
tcpdump -r <file>         # Read packets from file
tcpdump -c <count>        # Capture specific number of packets
```
