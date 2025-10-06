# Start-Process Command

`Start-Process` is a PowerShell command used to start one or more processes on the local computer.

## Common Options

| Option             | Explanation                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| `-FilePath`        | Specifies the program or document to start.                                 |
| `-ArgumentList`    | Specifies parameters or arguments to be passed to the started program.      |
| `-WorkingDirectory`| Sets the working directory for the process.                                 |
| `-NoNewWindow`     | Starts the process in the current window instead of a new one.              |
| `-Wait`            | Waits for the process to complete before moving to the next command.        |
| `-PassThru`        | Returns a process object for the started process.                           |
| `-Credential`      | Specifies a user account to run the process as a different user.            |

## Usage Examples

### Open Notepad
```powershell
Start-Process -FilePath "notepad.exe"
```

### Open a URL in Default Browser
```powershell
Start-Process -FilePath "https://www.example.com"
```

### Run a Script with Arguments
```powershell
Start-Process -FilePath "script.ps1" -ArgumentList "-param1 value1 -param2 value2"
```

### Start a Process and Wait for Completion
```powershell
Start-Process -FilePath "example.exe" -Wait
```

### Start a Process as a Different User
```powershell
$credential = Get-Credential
Start-Process -FilePath "notepad.exe" -Credential $credential
```

## Cheat Sheet

```plaintext
# Basic Usage
Start-Process -FilePath "<file>"

# With Arguments
Start-Process -FilePath "<file>" -ArgumentList "<args>"

# Specify Working Directory
Start-Process -FilePath "<file>" -WorkingDirectory "<path>"

# Wait for Completion
Start-Process -FilePath "<file>" -Wait

# Run as Different User
$cred = Get-Credential
Start-Process -FilePath "<file>" -Credential $cred
```

This guide provides a practical overview of `Start-Process` for common tasks in a concise manner.
