# Stop-Process Command

`Stop-Process` is a Windows PowerShell command used to terminate running processes. It's a useful tool for managing system resources and stopping unresponsive applications.

## Common Options

| Option                  | Description                                      |
|-------------------------|--------------------------------------------------|
| `-Name`                 | Specifies the process name to stop.              |
| `-Id`                   | Specifies the process ID to stop.                |
| `-Force`                | Forces the termination of a process.             |
| `-PassThru`             | Outputs information about the stopped process.   |
| `-WhatIf`               | Shows what would happen if the command runs.     |
| `-Confirm`              | Asks for confirmation before stopping a process. |

## Usage Examples

### Stop a Process by Name

```powershell
Stop-Process -Name "notepad"
```

### Stop a Process by ID

```powershell
Stop-Process -Id 1234
```

### Force Stop a Process

```powershell
Stop-Process -Name "notepad" -Force
```

### Display Information About Stopped Process

```powershell
Stop-Process -Name "notepad" -PassThru
```

### Simulate Stop-Process

```powershell
Stop-Process -Name "notepad" -WhatIf
```

## Cheat Sheet

```plaintext
Stop-Process -Name <ProcessName>
Stop-Process -Id <ProcessId>
Stop-Process -Name <ProcessName> -Force
Stop-Process -Name <ProcessName> -PassThru
Stop-Process -Name <ProcessName> -WhatIf
```
