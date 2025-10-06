# Get-Process Command Overview

`Get-Process` is a Windows PowerShell command that retrieves information about the processes running on a local or remote system. It provides details such as process names, IDs, CPU usage, and more.

## Common Options

| Option           | Explanation                                          |
|------------------|------------------------------------------------------|
| `-Name`          | Filters the processes by the specified name.         |
| `-Id`            | Filters the processes by the specified process ID.   |
| `-ComputerName`  | Specifies a remote computer to view processes on.    |
| `-FileVersionInfo` | Includes file version information for the processes. |
| `-Module`        | Includes the modules associated with the processes.  |

## Usage Examples

### List All Processes
```powershell
Get-Process
```

### Filter Processes by Name
```powershell
Get-Process -Name "notepad"
```

### Filter Processes by ID
```powershell
Get-Process -Id 1234
```

### Get Processes on a Remote Computer
```powershell
Get-Process -ComputerName "RemotePC"
```

### Include File Version Information
```powershell
Get-Process -Name "explorer" -FileVersionInfo
```

### Include Modules for a Specific Process
```powershell
Get-Process -Name "chrome" -Module
```

## Cheat Sheet

```markdown
# List all processes
Get-Process

# Filter by process name
Get-Process -Name "name"

# Filter by process ID
Get-Process -Id pid

# Check processes on a remote machine
Get-Process -ComputerName "remotePC"

# Include file info
Get-Process -Name "name" -FileVersionInfo

# Include modules
Get-Process -Name "name" -Module
```
