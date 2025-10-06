# Get-EventLog Command in Windows

`Get-EventLog` is a PowerShell cmdlet used to retrieve the entries from event logs on local and remote computers. It can be used for monitoring system, security, application events, and more.

## Common Options

| Option                     | Explanation                                                   |
|----------------------------|---------------------------------------------------------------|
| `-LogName <String>`        | Specifies the name of the event log to query.                 |
| `-Newest <Int32>`          | Retrieves the newest specified number of entries.             |
| `-EntryType <String[]>`    | Filters entries by type (Error, Warning, Information, etc.).  |
| `-InstanceId <Int64>`      | Filters entries by the event instance ID.                     |
| `-Message <String>`        | Filters entries by message text.                              |
| `-After <DateTime>`        | Selects entries after a specific date.                        |
| `-Before <DateTime>`       | Selects entries before a specific date.                       |
| `-ComputerName <String[]>` | Retrieves logs from remote computers.                         |

## Usage Examples

### Retrieve the Newest 10 Errors from the Application Log

```powershell
Get-EventLog -LogName Application -EntryType Error -Newest 10
```

### Retrieve Events with a Specific Instance ID

```powershell
Get-EventLog -LogName System -InstanceId 1234
```

### Retrieve Events from a Specific Date Range

```powershell
Get-EventLog -LogName Security -After "2023-10-01" -Before "2023-10-15"
```

### Retrieve Events from a Remote Computer

```powershell
Get-EventLog -LogName Application -ComputerName "RemotePC"
```

## Cheat Sheet

```powershell
# List newest 10 events from Application log
Get-EventLog -LogName Application -Newest 10

# Filter by Error in the System log
Get-EventLog -LogName System -EntryType Error

# Events from specific date range
Get-EventLog -LogName Security -After "YYYY-MM-DD" -Before "YYYY-MM-DD"

# Retrieve from remote machine
Get-EventLog -LogName Application -ComputerName "RemotePC"
```
