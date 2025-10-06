# `ifconfig` Command

The `ifconfig` command is used to configure, manage, and query network interface parameters in Linux. It is particularly useful for diagnosing and fixing network issues.

## Common Options

| Option           | Description                                           |
|------------------|-------------------------------------------------------|
| `interface`      | Specify the name of the network interface to configure. |
| `up`             | Activate the specified network interface.             |
| `down`           | Deactivate the specified network interface.           |
| `inet addr`      | Assign an IP address to the interface.                |
| `netmask`        | Set the network mask for the interface.               |
| `broadcast`      | Set the broadcast address for the interface.          |
| `mtu`            | Set the Maximum Transmission Unit (MTU) size.         |

## Usage Examples

### Activate a Network Interface

```bash
sudo ifconfig eth0 up
```

### Deactivate a Network Interface

```bash
sudo ifconfig eth0 down
```

### Assign an IP Address

```bash
sudo ifconfig eth0 192.168.1.10
```

### Set IP Address with Netmask

```bash
sudo ifconfig eth0 192.168.1.10 netmask 255.255.255.0
```

### Set Broadcast Address

```bash
sudo ifconfig eth0 broadcast 192.168.1.255
```

### Change MTU Size

```bash
sudo ifconfig eth0 mtu 1400
```

## Compact Cheat Sheet

```plaintext
# Activate interface
sudo ifconfig <interface> up

# Deactivate interface
sudo ifconfig <interface> down

# Set IP address
sudo ifconfig <interface> <ip-address>

# Set IP and Netmask
sudo ifconfig <interface> <ip-address> netmask <netmask>

# Set Broadcast
sudo ifconfig <interface> broadcast <broadcast-address>

# Set MTU
sudo ifconfig <interface> mtu <size>
```

Note: Use `ifconfig` primarily on older systems. On modern distributions, consider using `ip` commands as `ifconfig` may be deprecated.
