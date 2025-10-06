# Test-NetConnection Command

`Test-NetConnection` is a versatile Windows PowerShell cmdlet used for diagnosing network connectivity issues. It can perform tests such as ping, traceroute, and port checking.

## Common Options

| Option                | Description                                                         |
|-----------------------|---------------------------------------------------------------------|
| `-ComputerName`       | Specifies the remote computer or IP address to test connectivity.   |
| `-Port`               | Checks the connectivity to a specific port on the target computer.  |
| `-InformationLevel`   | Defines the level of information returned (default, detailed).      |
| `-TraceRoute`         | Performs a traceroute to the specified computer.                    |
| `-CommonTCPPort`      | Tests predefined common TCP ports (e.g., HTTP, RDP).                |

## Usage Examples

### Basic Ping Test

```powershell
Test-NetConnection -ComputerName google.com
```

### Check Port Connectivity

```powershell
Test-NetConnection -ComputerName example.com -Port 80
```

### Detailed Information with Traceroute

```powershell
Test-NetConnection -ComputerName example.com -InformationLevel Detailed -TraceRoute
```

### Test Common TCP Port (e.g., HTTP)

```powershell
Test-NetConnection -ComputerName example.com -CommonTCPPort HTTP
```

## Cheat Sheet

```plaintext
# Basic connectivity test
Test-NetConnection -ComputerName <hostname_or_ip>

# Check specific port
Test-NetConnection -ComputerName <hostname_or_ip> -Port <port_number>

# Traceroute with details
Test-NetConnection -ComputerName <hostname_or_ip> -InformationLevel Detailed -TraceRoute

# Test common TCP port (e.g., HTTP, RDP)
Test-NetConnection -ComputerName <hostname_or_ip> -CommonTCPPort <port_name>
```
