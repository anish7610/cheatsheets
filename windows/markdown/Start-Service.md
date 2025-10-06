# Start-Service Command

The `Start-Service` command in Windows PowerShell is used to start services on a local or remote computer. It's useful for managing system and application services.

## Common Options

| Option           | Description                                  |
|------------------|----------------------------------------------|
| `-Name`          | Specifies the service name to start.         |
| `-DisplayName`   | Specifies the display name of the service.   |
| `-InputObject`   | Accepts a service object for starting.       |
| `-PassThru`      | Returns the service object after starting.   |
| `-Verbose`       | Provides detailed information during execution. |

## Usage Examples

### Start a Service by Name

Start the "Print Spooler" service by name:
```bash
Start-Service -Name "Spooler"
```

### Start a Service by Display Name

Start a service using its display name:
```bash
Start-Service -DisplayName "Print Spooler"
```

### Start a Service with Detailed Output

Start a service and get detailed output:
```bash
Start-Service -Name "Spooler" -Verbose
```

### Start Multiple Services

Start multiple services:
```bash
"Spooler", "wuauserv" | ForEach-Object { Start-Service -Name $_ }
```

## Cheat Sheet

```plaintext
# Start a service by name
Start-Service -Name "ServiceName"

# Start a service by display name
Start-Service -DisplayName "Service Display Name"

# Start with detailed output
Start-Service -Name "ServiceName" -Verbose

# Start multiple services
"Service1", "Service2" | ForEach-Object { Start-Service -Name $_ }
```
