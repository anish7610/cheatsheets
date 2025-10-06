# Get-WinEvent Command in Windows

`Get-WinEvent` is a PowerShell command used to retrieve Windows event logs. The `-LogName Security` parameter specifies the Security log, commonly used for monitoring security-related events.

## Common Options

| Option                    | Description                                                      |
|---------------------------|------------------------------------------------------------------|
| `-LogName`                | Specifies the name of the event log (e.g., Security, System).    |
| `-MaxEvents`              | Limits the number of events returned.                            |
| `-FilterHashtable`        | Allows filtering events using a hashtable for more precise queries. |
| `-Oldest`                 | Retrieves events from the oldest to the newest.                  |
| `-ComputerName`           | Accesses event logs from a remote computer.                      |

## Usage Examples

### Retrieve Recent Security Events
```powershell
Get-WinEvent -LogName Security -MaxEvents 10
```

### Filter Events by Event ID
```powershell
Get-WinEvent -LogName Security -FilterHashtable @{Id=4625}
```

### Accessing Security Logs from a Remote Computer
```powershell
Get-WinEvent -LogName Security -ComputerName RemotePC
```

### Retrieve Events from Oldest to Newest
```powershell
Get-WinEvent -LogName Security -Oldest | Select-Object -First 5
```

## Cheat Sheet

```plaintext
# View the latest 10 security events
Get-WinEvent -LogName Security -MaxEvents 10

# Filter events by a specific event ID
Get-WinEvent -LogName Security -FilterHashtable @{Id=4625}

# Get security logs from a remote machine
Get-WinEvent -LogName Security -ComputerName <RemotePC>

# Retrieve events in chronological order
Get-WinEvent -LogName Security -Oldest
```
