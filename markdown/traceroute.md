# `traceroute` Command in Linux

The `traceroute` command in Linux is used to display the route packets take to reach a network host. It helps in diagnosing and understanding network paths and pinpointing where delays occur.

## Common Options

| Option     | Description                                                                 |
|------------|-----------------------------------------------------------------------------|
| `-m`       | Specifies the maximum number of hops (TTL).                                  |
| `-n`       | Prevents DNS resolution for hostnames, showing raw IP addresses.             |
| `-p`       | Sets the base UDP port number for outgoing packets.                          |
| `-q`       | Specifies the number of probe queries per hop.                               |
| `-w`       | Sets the timeout for each probe in seconds.                                  |
| `-I`       | Uses ICMP ECHO instead of UDP datagrams (like `ping`).                       |

## Usage Examples

### Trace Route to a Host
```bash
traceroute google.com
```

### Limit Maximum Hops to 10
```bash
traceroute -m 10 google.com
```

### Show IP Addresses Only
```bash
traceroute -n google.com
```

### Use ICMP ECHO
```bash
traceroute -I google.com
```

### Set Specific Timeout
```bash
traceroute -w 2 google.com
```

## Cheat Sheet

```markdown
# Basic Usage
traceroute [OPTIONS] HOST

# Common Examples
traceroute google.com             # Trace route to Google
traceroute -n example.com         # Disable DNS resolution
traceroute -m 10 example.com      # Limit to 10 hops
traceroute -I example.com         # Use ICMP ECHO

# Quick Reference for Options
-m N    # Max hops
-n      # Numeric IP output
-I      # Use ICMP
```

Keep this as a handy reference to effectively use the `traceroute` command for network diagnostics and troubleshooting.
