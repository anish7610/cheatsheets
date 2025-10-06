# Get-NetUDPEndpoint Command

The `Get-NetUDPEndpoint` command in Windows PowerShell is used to retrieve information about UDP network endpoints on the system. It lists various details such as local addresses, remote addresses, and port numbers.

## Common Options

| Option                  | Description                                                                        |
|-------------------------|------------------------------------------------------------------------------------|
| `-LocalAddress`         | Filters results by the specified local IP address.                                 |
| `-LocalPort`            | Filters results by the specified local UDP port.                                   |
| `-RemoteAddress`        | Filters results by the specified remote IP address.                                |
| `-RemotePort`           | Filters results by the specified remote UDP port.                                  |
| `-State`                | Filters results by the state of the connection (e.g., Bound, Listening).           |

## Usage Examples

### List All UDP Endpoints
```bash
Get-NetUDPEndpoint
```

### Filter by Local Port
```bash
Get-NetUDPEndpoint -LocalPort 80
```

### Filter by Local Address
```bash
Get-NetUDPEndpoint -LocalAddress "192.168.1.10"
```

### Filter by Remote Address and Port
```bash
Get-NetUDPEndpoint -RemoteAddress "10.0.0.5" -RemotePort 53
```

### Display Specific Properties
```bash
Get-NetUDPEndpoint | Select-Object LocalAddress, LocalPort, RemoteAddress
```

## Cheat Sheet

```plaintext
# List all UDP endpoints
Get-NetUDPEndpoint

# Filter by local port
Get-NetUDPEndpoint -LocalPort <PortNumber>

# Filter by local address
Get-NetUDPEndpoint -LocalAddress <IPAddress>

# Filter by remote address and port
Get-NetUDPEndpoint -RemoteAddress <IPAddress> -RemotePort <PortNumber>

# Select specific properties
Get-NetUDPEndpoint | Select-Object <Property1>, <Property2>
```
