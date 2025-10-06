## `nload` Command

### Description

`nload` is a command-line tool for monitoring network traffic in real-time. It provides a visual representation of incoming and outgoing data rates on network interfaces.

### Common Options

| Option    | Description                               |
|-----------|-------------------------------------------|
| `-a <seconds>` | Sets the length of the displayed network history (default: 300). |
| `-i <device>`  | Specifies which network device to monitor (e.g., eth0, wlan0). |
| `-t <milliseconds>` | Sets the refresh interval (default: 500ms). |
| `-m`         | Shows multiple devices at once.  |
| `-u <h|b|k|m|g>` | Sets the unit to display data (h: human-readable, b: bytes, k: kilobytes, m: megabytes, g: gigabytes). |

### Usage Examples

#### Example 1: Monitor a Specific Interface
Monitor traffic on the `eth0` interface.

```bash
nload -i eth0
```

#### Example 2: Set Data Display Unit
Display data in kilobytes for `wlan0`.

```bash
nload -i wlan0 -u k
```

#### Example 3: Display All Interfaces
Show data transfer for all interfaces.

```bash
nload -m
```

#### Example 4: Adjust Refresh Rate
Change refresh rate to 1 second (1000 milliseconds).

```bash
nload -t 1000
```

### Quick Reference Cheat Sheet

```plaintext
nload -i <device>   # Monitor specific interface
nload -m            # Monitor all interfaces
nload -u k          # Display data in kilobytes
```
