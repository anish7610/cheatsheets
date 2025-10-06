### Description

The `Get-WinEvent -LogName System` command is used in Windows PowerShell to retrieve and display event logs from the System event log. It's helpful for diagnosing system issues and monitoring system events.

### Common Options

| Option                      | Explanation                                               |
|-----------------------------|-----------------------------------------------------------|
| `-MaxEvents <Int32>`        | Limits the number of events returned.                     |
| `-FilterXPath <XPath>`      | Filters log entries using XPath query syntax.             |
| `-FilterHashtable <Hash>`   | Uses a hashtable to filter events (e.g., by ID or source).|
| `-Oldest`                   | Displays logs starting from the oldest entry.             |

### Usage Examples

```powershell
# Retrieve the latest 10 events from the System log
Get-WinEvent -LogName System -MaxEvents 10

# Retrieve events from the System log with a specific Event ID
Get-WinEvent -LogName System -FilterHashtable @{LogName='System'; Id=7001}

# Retrieve events from the System log sorted from oldest to newest
Get-WinEvent -LogName System -Oldest

# Filter System log events using XPath
Get-WinEvent -LogName System -FilterXPath "*[System/EventID=7036]"
```

### Cheat Sheet

```plaintext
# Basic command
Get-WinEvent -LogName System

# Limit results
-MaxEvents <Int32>

# Specific Event ID
-FilterHashtable @{LogName='System'; Id=<EventID>}

# Sorted from oldest
-Oldest

# XPath filtering example
-FilterXPath "*[System/EventID=<ID>]"
```
