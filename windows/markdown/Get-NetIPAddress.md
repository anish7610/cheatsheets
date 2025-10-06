# Get-NetIPAddress Command

`Get-NetIPAddress` is a PowerShell command used to retrieve IP address configuration details on a Windows machine.

## Common Options

| Option                    | Description                                         |
|---------------------------|-----------------------------------------------------|
| `-InterfaceAlias`         | Filter results by network interface name.           |
| `-AddressFamily`          | Filter by address family: IPv4 or IPv6.             |
| `-IPAddress`              | Get details for a specific IP address.              |
| `-InterfaceIndex`         | Filter by network interface index number.           |
| `-PrefixLength`           | Filter by subnet prefix length.                     |

## Usage Examples

### Get All IP Addresses
```powershell
Get-NetIPAddress
```

### Filter by Interface Name
```powershell
Get-NetIPAddress -InterfaceAlias "Ethernet"
```

### Retrieve Only IPv4 Addresses
```powershell
Get-NetIPAddress -AddressFamily IPv4
```

### Get Specific IP Address Details
```powershell
Get-NetIPAddress -IPAddress 192.168.1.1
```

### Filter by Interface Index
```powershell
Get-NetIPAddress -InterfaceIndex 12
```

## Cheat Sheet

```markdown
# Get all IP addresses
Get-NetIPAddress

# Filter by interface name
Get-NetIPAddress -InterfaceAlias "Name"

# Filter by IPv4 only
Get-NetIPAddress -AddressFamily IPv4

# Get specific IP address details
Get-NetIPAddress -IPAddress x.x.x.x
```
