## Description

`Remove-EventLog` is a PowerShell command used to delete event logs on a Windows machine. It is useful for clearing old logs or when reorganizing log settings.

## Common Options

| Option                | Explanation                                           |
|-----------------------|-------------------------------------------------------|
| `-LogName`            | Specifies the name of the event log to be removed.    |
| `-ComputerName`       | Specifies a remote computer for removing event logs.  |
| `-WhatIf`             | Shows what would happen if the command runs, without executing it. |
| `-Confirm`            | Prompts for confirmation before executing the command. |

## Usage Examples

### Remove a Local Event Log

```powershell
Remove-EventLog -LogName "Application"
```

### Remove a Specific Log on a Remote Computer

```powershell
Remove-EventLog -LogName "Security" -ComputerName "RemotePC"
```

### Preview the Command Without Executing

```powershell
Remove-EventLog -LogName "System" -WhatIf
```

### Remove the Log with Confirmation Prompt

```powershell
Remove-EventLog -LogName "Setup" -Confirm
```

## Cheat Sheet

```plaintext
Remove-EventLog -LogName <LogName> [-ComputerName <Name>] [-WhatIf] [-Confirm]
```
