# Clear-EventLog Command

`Clear-EventLog` is a Windows PowerShell command used to delete all entries from specified event logs on a local or remote computer. This is useful for maintaining log cleanliness and managing disk space.

## Common Options

| Option                  | Description                                                                    |
|-------------------------|--------------------------------------------------------------------------------|
| `-LogName`              | Specifies the name of the event log to clear. Multiple log names can be given. |
| `-ComputerName`         | Names of the remote computers where the event logs should be cleared.          |
| `-Confirm`              | Prompts for confirmation before clearing the logs.                             |
| `-WhatIf`               | Shows what would happen if the command runs, without executing it.             |

## Usage Examples

### Clear a Single Log
```powershell
Clear-EventLog -LogName "Application"
```

### Clear Multiple Logs
```powershell
Clear-EventLog -LogName "System", "Security"
```

### Clear Logs on a Remote Computer
```powershell
Clear-EventLog -LogName "Application" -ComputerName "RemotePC"
```

### Confirm Before Clearing
```powershell
Clear-EventLog -LogName "Application" -Confirm
```

## Cheat Sheet

```markdown
# Clear specific log
Clear-EventLog -LogName "LogName"

# Clear multiple logs
Clear-EventLog -LogName "Log1", "Log2"

# Clear log on remote machine
Clear-EventLog -LogName "LogName" -ComputerName "RemotePC"

# Prompt before clearing
Clear-EventLog -LogName "LogName" -Confirm

# Simulate clearing without execution
Clear-EventLog -LogName "LogName" -WhatIf
```

Keep this guide handy for quick operations with `Clear-EventLog`.
