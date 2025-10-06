# `iftop` Command Overview

`iftop` is a network monitoring tool that displays bandwidth usage on a network interface. It shows a real-time view of data flowing in and out of your machine, giving a snapshot of current connections and their bandwidth consumption.

## Common Options

| Option       | Explanation                                               |
|--------------|-----------------------------------------------------------|
| `-i <iface>` | Specify the network interface to monitor.                 |
| `-B`         | Display bandwidth in bytes instead of bits.               |
| `-n`         | Show numerical addresses instead of resolving hostnames.  |
| `-N`         | Do not resolve port numbers to service names.             |
| `-P`         | Show ports along with host addresses.                     |
| `-t`         | Use a text interface rather than curses.                  |
| `-f <filter>`| Apply a pcap-style filter to select traffic to display.   |

## Usage Examples

### Monitor a Specific Interface

To monitor the `eth0` interface:

```bash
sudo iftop -i eth0
```

### Display Bandwidth in Bytes

To view bandwidth usage in bytes instead of bits:

```bash
sudo iftop -B
```

### Show Only Numerical Addresses and Ports

To avoid resolving hostnames and port numbers:

```bash
sudo iftop -nN
```

### Filter Traffic by Port

To display only traffic on port 80:

```bash
sudo iftop -f "port 80"
```

## Cheat Sheet

```plaintext
sudo iftop -i <interface>         # Monitor specific interface
sudo iftop -B                     # Show in bytes
sudo iftop -nN                    # Show numerical IPs and ports
sudo iftop -f "port <num>"        # Filter by port
```
