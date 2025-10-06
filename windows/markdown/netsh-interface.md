# `netsh interface`

The `netsh interface` command in Windows is used to configure and manage network interfaces. It allows for various network-related tasks such as assigning IP addresses, changing network interface settings, and more.

## Common Options

| Option                  | Explanation                                          |
|-------------------------|------------------------------------------------------|
| `show interfaces`       | Displays a list of all network interfaces.           |
| `show interface "name"` | Shows detailed information about a specific interface.|
| `set interface`         | Modifies an interface property like enabling/disabling.|
| `ip set address`        | Assigns an IP address to an interface.               |
| `ip add dns`            | Sets a DNS server for a network interface.           |
| `ip delete dns`         | Removes a DNS server entry for a network interface.  |

## Usage Examples

### Display All Network Interfaces

```bash
netsh interface show interfaces
```

### Show Details for a Specific Interface

```bash
netsh interface show interface "Ethernet"
```

### Enable a Network Interface

```bash
netsh interface set interface "Ethernet" admin=enable
```

### Assign a Static IP Address

```bash
netsh interface ip set address name="Ethernet" static 192.168.1.10 255.255.255.0 192.168.1.1
```

### Add a DNS Server

```bash
netsh interface ip add dns name="Ethernet" 8.8.8.8 index=1
```

### Remove a DNS Server

```bash
netsh interface ip delete dns name="Ethernet" 8.8.8.8
```

## Cheat Sheet

```plaintext
# Show interfaces
netsh interface show interfaces

# Show specific interface
netsh interface show interface "name"

# Enable/Disable interface
netsh interface set interface "name" admin=enable/disable

# Set static IP
netsh interface ip set address name="name" static IP MASK GATEWAY

# Add DNS server
netsh interface ip add dns name="name" DNS

# Delete DNS server
netsh interface ip delete dns name="name" DNS
```
