# Write-EventLog Command

`Write-EventLog` is a Windows PowerShell command used to write events to an event log on a local or remote computer. It enables users to specify details such as the event message, event source, and event ID.

## Common Options

| Option          | Explanation                                             |
|-----------------|---------------------------------------------------------|
| `-LogName`      | The name of the event log to write to (e.g., "Application"). |
| `-Source`       | The source of the event, typically the app or service writing the event. |
| `-EventID`      | A numeric identifier for the event (normally between 1 and 65535). |
| `-Message`      | Descriptive text about the event.                        |
| `-EntryType`    | Type of event: Information, Warning, Error, etc.         |
| `-Category`     | A numeric category to describe the event (optional).     |

## Usage Examples

### Write an Information Event
```powershell
Write-EventLog -LogName "Application" -Source "MyApp" -EventID 1001 -EntryType Information -Message "MyApp has started successfully."
```

### Write an Error Event
```powershell
Write-EventLog -LogName "Application" -Source "MyApp" -EventID 1002 -EntryType Error -Message "MyApp encountered an error during execution."
```

### Write a Warning Event
```powershell
Write-EventLog -LogName "System" -Source "MyService" -EventID 2001 -EntryType Warning -Message "Low disk space warning."
```

## Cheat Sheet

```plaintext
# Write an event to Application log
Write-EventLog -LogName "Application" -Source "SourceName" -EventID 1000 -EntryType Type -Message "Your message"
```

Replace `SourceName`, `Type` (Information, Warning, Error), and `Your message` with your specifics.
