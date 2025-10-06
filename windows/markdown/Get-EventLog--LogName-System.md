# Get-EventLog Command Overview

`Get-EventLog -LogName System` is a PowerShell command used to retrieve entries from the Windows event log, specifically targeting the "System" log. This helps in monitoring and troubleshooting system and hardware events.

## Common Options

| Option             | Explanation                                                                               |
|--------------------|-------------------------------------------------------------------------------------------|
| `-Newest`          | Retrieves the most recent entries.                                                        |
| `-EntryType`       | Filters entries by type, such as `Error`, `Warning`, or `Information`.                    |
| `-InstanceId`      | Gets entries with a specific event instance ID.                                           |
| `-Source`          | Filters by the source of the event log entry (e.g., "Service Control Manager").           |
| `-Before`          | Retrieves entries before a specified date and time.                                       |
| `-After`           | Retrieves entries after a specified date and time.                                        |
| `-ComputerName`    | Specifies a remote computer to query.                                                     |
| `-UserName`        | Filters entries based on the user responsible for the event.                              |

## Usage Examples

### Retrieve the 10 Most Recent System Events

```powershell
Get-EventLog -LogName System -Newest 10
```

### Filter by EntryType: Errors and Warnings Only

```powershell
Get-EventLog -LogName System -EntryType Error, Warning
```

### Find Events from a Specific Source

```powershell
Get-EventLog -LogName System -Source "Service Control Manager"
```

### Get Events Before a Specific Date

```powershell
Get-EventLog -LogName System -Before (Get-Date).AddDays(-7)
```

### Access Remote System Log

```powershell
Get-EventLog -LogName System -ComputerName "RemotePC"
```

## Cheat Sheet

```plaintext
# Get recent events
Get-EventLog -LogName System -Newest <Number>

# Filter by type
Get-EventLog -LogName System -EntryType Error, Warning

# Specific source
Get-EventLog -LogName System -Source "<SourceName>"

# Date filtering
Get-EventLog -LogName System -Before (Get-Date).AddDays(-<Days>)

# Remote access
Get-EventLog -LogName System -ComputerName "<ComputerName>"
```

Use these examples and the table as a quick reference for common use cases.
