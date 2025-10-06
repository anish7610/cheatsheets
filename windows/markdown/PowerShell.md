# PowerShell Overview

PowerShell is a task automation and configuration management framework from Microsoft, consisting of a command-line shell and the associated scripting language.

## Common Options

| Option / Cmdlet     | Description                                               |
|---------------------|-----------------------------------------------------------|
| `Get-Help`          | Displays help information for cmdlets and scripts.        |
| `Get-Command`       | Lists all available cmdlets and functions.                |
| `Get-Process`       | Retrieves information about running processes.            |
| `Stop-Process`      | Stops a running process by its ID or name.                |
| `Get-Service`       | Lists the status of services on a system.                 |
| `Start-Service`     | Starts a stopped service.                                 |
| `Stop-Service`      | Stops a running service.                                  |
| `Set-Location`      | Changes the current working directory.                    |
| `Copy-Item`         | Copies an item from one location to another.              |
| `Remove-Item`       | Deletes files or directories.                             |
| `Get-Content`       | Retrieves the content of a file.                          |
| `Set-Content`       | Writes content to a file, replacing existing content.     |
| `Add-Content`       | Appends content to the end of a file.                     |

## Usage Examples

### List Processes

```powershell
Get-Process
```

### Stop a Process by Name

```powershell
Stop-Process -Name "notepad"
```

### Get Service Status

```powershell
Get-Service
```

### Copy a File

```powershell
Copy-Item -Path "C:\example.txt" -Destination "D:\backup\example.txt"
```

### Change Directory

```powershell
Set-Location -Path "C:\Users"
```

### View File Content

```powershell
Get-Content -Path "C:\example.txt"
```

## Cheat Sheet

```plaintext
Get-Help <cmdlet>      # Show help
Get-Command            # List commands
Get-Process            # List processes
Stop-Process -Name <name> # Stop process
Get-Service            # List services
Start-Service <name>   # Start service
Stop-Service <name>    # Stop service
Set-Location <path>    # Change directory
Copy-Item <src> <dst>  # Copy file
Remove-Item <path>     # Delete file
Get-Content <file>     # View file
Set-Content <file> -Value <text> # Write file
Add-Content <file> -Value <text> # Append file
```
