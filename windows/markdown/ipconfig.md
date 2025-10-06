# `ipconfig` Command in Windows

## Description
`ipconfig` is a command-line utility in Windows that displays the current network configuration details, including IP address, subnet mask, and default gateway for each network adapter.

## Common Options

| Option         | Description                                       |
|----------------|---------------------------------------------------|
| `/all`         | Displays detailed information for all adapters.   |
| `/release`     | Releases the current IP address for all adapters. |
| `/renew`       | Renews the IP address for all adapters.           |
| `/flushdns`    | Clears the DNS resolver cache.                    |
| `/displaydns`  | Displays the contents of the DNS resolver cache.  |

## Usage Examples

### Display Basic IP Configuration
```shell
ipconfig
```

### Display Detailed Information for All Adapters
```shell
ipconfig /all
```

### Release and Renew IP Address for All Adapters
```shell
ipconfig /release
ipconfig /renew
```

### Flush DNS Resolver Cache
```shell
ipconfig /flushdns
```

### Display DNS Resolver Cache
```shell
ipconfig /displaydns
```

## Cheat Sheet

```plaintext
ipconfig           # Display IP configuration
ipconfig /all      # Detailed adapter info
ipconfig /release  # Release IP address
ipconfig /renew    # Renew IP address
ipconfig /flushdns # Clear DNS cache
ipconfig /displaydns # Show DNS cache
```
