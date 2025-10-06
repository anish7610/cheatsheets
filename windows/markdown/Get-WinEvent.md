# `Get-WinEvent`

`Get-WinEvent` is a Windows PowerShell cmdlet used to query event logs and event tracing logs. It's a powerful tool for system administrators to monitor and analyze system, security, and application events.

## Common Options

| Option                  | Description                                                  |
|-------------------------|--------------------------------------------------------------|
| `-LogName <string>`     | Specifies the log name, e.g., "System", "Application".       |
| `-ProviderName <string>`| Filters events by provider name.                             |
| `-MaxEvents <int>`      | Limits the number of events returned.                        |
| `-FilterHashTable`      | Allows more refined querying with hash tables.               |
| `-Oldest`               | Displays the oldest events first (default shows newest).     |
| `-ComputerName <string>` | Queries events from a remote computer.                      |

## Usage Examples

### Retrieve Events from the System Log

```powershell
Get-WinEvent -LogName System -MaxEvents 10
```

### Retrieve Events with a Specific Provider

```powershell
Get-WinEvent -ProviderName Microsoft-Windows-Winlogon
```

### Filter Events by ID and Log Name

```powershell
Get-WinEvent -FilterHashTable @{LogName="System"; Id=6006} -MaxEvents 5
```

### Query Events from a Remote Computer

```powershell
Get-WinEvent -LogName Application -ComputerName RemotePC -MaxEvents 10
```

## Cheat Sheet

```plaintext
Get-WinEvent -LogName <LogName> -MaxEvents <n>
Get-WinEvent -ProviderName <ProviderName>
Get-WinEvent -FilterHashTable @{LogName=<LogName>; Id=<EventId>}
Get-WinEvent -LogName <LogName> -ComputerName <RemotePC>
```
