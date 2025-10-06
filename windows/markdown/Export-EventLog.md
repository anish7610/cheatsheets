# Export-EventLog Command

`Export-EventLog` is a PowerShell cmdlet used to export entries from an event log on a local or remote computer to a file in `*.evt` or `*.evtx` format.

## Common Options

| Option                | Description                                                        |
|-----------------------|--------------------------------------------------------------------|
| `-LogName`            | Specifies the event log name to export (e.g., Application, System).|
| `-FilePath`           | Defines the path and filename for the exported event log file.     |
| `-ComputerName`       | Indicates the remote computer from which to export the event log.  |
| `-Newest`             | Exports a specified number of the most recent events.              |
| `-UserName`           | Specifies credentials when accessing a remote computer.            |

## Usage Examples

### Export System Log to File

```powershell
Export-EventLog -LogName System -FilePath C:\Logs\SystemLog.evt
```

### Export Application Log from Remote Computer

```powershell
Export-EventLog -LogName Application -FilePath C:\Logs\AppLog.evt -ComputerName Server01
```

### Export the 50 Most Recent Entries

```powershell
Export-EventLog -LogName Security -FilePath C:\Logs\SecurityLog.evt -Newest 50
```

## Cheat Sheet

```plaintext
# Export all system logs
Export-EventLog -LogName System -FilePath <path>

# Export logs from remote machine
Export-EventLog -LogName <LogName> -FilePath <path> -ComputerName <RemotePC>

# Export recent X entries
Export-EventLog -LogName <LogName> -FilePath <path> -Newest <Number>
```
