# `iptables` Command Overview

`iptables` is a command-line utility for configuring and managing packet filtering rules in the Linux kernel firewall. It is used to define rules that control the processing and forwarding of network traffic.

## Common Options

| Option      | Description                                                       |
|-------------|-------------------------------------------------------------------|
| `-A`        | Append a rule to a chain                                          |
| `-D`        | Delete a rule from a chain                                        |
| `-I`        | Insert a rule at a specific position in a chain                   |
| `-L`        | List all rules in a chain                                         |
| `-F`        | Flush all rules in a chain                                        |
| `-P`        | Set the default policy for a chain (e.g., ACCEPT, DROP)           |
| `-N`        | Create a new chain                                                |
| `-X`        | Delete a user-defined chain                                       |
| `-v`        | Verbose output                                                    |
| `-n`        | Numeric output of addresses and ports (no DNS lookup)             |
| `--sport`   | Source port                                                       |
| `--dport`   | Destination port                                                  |
| `-s`        | Source address                                                    |
| `-d`        | Destination address                                               |
| `-j`        | Jump to the target action (e.g., ACCEPT, DROP, REJECT)            |

## Usage Examples

### Allow Incoming SSH Traffic
```bash
sudo iptables -A INPUT -p tcp --dport 22 -j ACCEPT
```

### Block Incoming Traffic from a Specific IP
```bash
sudo iptables -A INPUT -s 192.168.1.100 -j DROP
```

### List All Rules with Verbose Output
```bash
sudo iptables -L -v
```

### Flush All Rules in the INPUT Chain
```bash
sudo iptables -F INPUT
```

### Set Default Policy to DROP for the FORWARD Chain
```bash
sudo iptables -P FORWARD DROP
```

## Cheat Sheet

```plaintext
# Append rule to INPUT chain
iptables -A INPUT -p <protocol> --dport <port> -j <ACTION>

# Delete rule from INPUT chain by number
iptables -D INPUT <num>

# List all rules with numbers
iptables -L -v --line-numbers

# Flush all rules in INPUT chain
iptables -F INPUT

# Set default chain policy
iptables -P FORWARD DROP
```
