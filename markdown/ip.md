# Overview of `ip` Command

The `ip` command in Linux is a powerful tool used for network configuration and management. It replaces older tools like `ifconfig` and is part of the `iproute2` suite. It allows you to configure IP addresses, routes, link properties, and more.

## Common Options

| Option             | Description                                       |
|--------------------|---------------------------------------------------|
| `ip addr`          | Display or manage IP addresses                    |
| `ip link`          | Display or manage network interfaces              |
| `ip route`         | Display or manage routing table                   |
| `ip neigh`         | Display or manage ARP table entries               |
| `ip -s link`       | Display statistics for network interfaces         |
| `ip addr add`      | Add an IP address to an interface                 |
| `ip addr del`      | Remove an IP address from an interface            |
| `ip link set`      | Enable or disable a network interface             |
| `ip route add`     | Add a new route to the routing table              |
| `ip route del`     | Remove a route from the routing table             |

## Usage Examples

### Display IP Addresses

```bash
ip addr show
```

### Add an IP Address

```bash
ip addr add 192.168.1.100/24 dev eth0
```

### Remove an IP Address

```bash
ip addr del 192.168.1.100/24 dev eth0
```

### Bring a Network Interface Up

```bash
ip link set eth0 up
```

### Bring a Network Interface Down

```bash
ip link set eth0 down
```

### Display the Routing Table

```bash
ip route show
```

### Add a Route

```bash
ip route add 192.168.2.0/24 via 192.168.1.1
```

### Delete a Route

```bash
ip route del 192.168.2.0/24
```

## Quick Reference Cheat Sheet

```plaintext
ip addr show                # List IP addresses
ip link show                # List network interfaces
ip route show               # Show routing table
ip addr add [IP/CIDR] dev [IFACE]    # Add IP to interface
ip addr del [IP/CIDR] dev [IFACE]    # Remove IP from interface
ip link set [IFACE] up      # Bring interface up
ip link set [IFACE] down    # Bring interface down
ip route add [NET/CIDR] via [GATEWAY] # Add route
ip route del [NET/CIDR]     # Delete route
```
