# Get-NetTCPConnection Command

`Get-NetTCPConnection` is a PowerShell command used to retrieve information about current TCP connections on a Windows machine. It helps in network diagnostics and monitoring.

## Common Options

| Option               | Explanation                                     |
|----------------------|-------------------------------------------------|
| `-State`             | Filter connections by TCP state (e.g., Established, Listen). |
| `-LocalAddress`      | Filter results by local IP address.          |
| `-RemoteAddress`     | Filter results by remote IP address.         |
| `-LocalPort`         | Filter connections by local port number.     |
| `-RemotePort`        | Filter connections by remote port number.    |

## Usage Examples

### List all established TCP connections
```powershell
Get-NetTCPConnection -State Established
```

### Filter connections to a specific local IP
```powershell
Get-NetTCPConnection -LocalAddress 192.168.1.10
```

### Display connections on a specific local port
```powershell
Get-NetTCPConnection -LocalPort 80
```

### Find connections to a specific remote address
```powershell
Get-NetTCPConnection -RemoteAddress 10.0.0.5
```

### Show listening ports
```powershell
Get-NetTCPConnection -State Listen
```

## Cheat Sheet

```plaintext
# List all TCP connections
Get-NetTCPConnection

# Filter by state
Get-NetTCPConnection -State Established

# Filter by local address
Get-NetTCPConnection -LocalAddress <LocalIPAddress>

# Filter by local port
Get-NetTCPConnection -LocalPort <LocalPortNumber>

# Show listening connections
Get-NetTCPConnection -State Listen
```
