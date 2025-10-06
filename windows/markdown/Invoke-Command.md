# Invoke-Command Cheat Sheet

## Description

`Invoke-Command` in Windows PowerShell is used to run commands on local or remote computers. It allows for executing scripts or command blocks remotely, making it essential for managing multiple systems.

## Common Options

| Option                  | Description                                                      |
|-------------------------|------------------------------------------------------------------|
| `-ScriptBlock`          | Specifies the command or script block to run.                    |
| `-ComputerName`         | Specifies the remote computer(s) to run the command on.          |
| `-Credential`           | Provides user credentials for authentication on the remote system.|
| `-FilePath`             | Executes a script file rather than a command block.              |
| `-Session`              | Uses an existing session for the command.                        |
| `-ArgumentList`         | Supplies arguments to the script or command.                     |
| `-ThrottleLimit`        | Limits the number of concurrent connections.                     |

## Usage Examples

### Run a Command on a Remote Computer

```powershell
Invoke-Command -ComputerName "Server01" -ScriptBlock { Get-Process }
```

### Execute a Script File Remotely

```powershell
Invoke-Command -ComputerName "Server01" -FilePath "C:\Scripts\Update.ps1"
```

### Use Specific Credentials

```powershell
$cred = Get-Credential
Invoke-Command -ComputerName "Server01" -ScriptBlock { Get-Service } -Credential $cred
```

### Run with Arguments

```powershell
Invoke-Command -ComputerName "Server01" -ScriptBlock { param($name) Get-Service $name } -ArgumentList "W32Time"
```

### Run on Multiple Computers

```powershell
Invoke-Command -ComputerName "Server01","Server02" -ScriptBlock { Get-Date }
```

### Use an Existing Session

```powershell
$session = New-PSSession -ComputerName "Server01"
Invoke-Command -Session $session -ScriptBlock { Get-HotFix }
```

## Quick Reference

```plaintext
Invoke-Command -ComputerName <Name> -ScriptBlock { <Command> } [-Credential <User>]
Invoke-Command -FilePath <Path> [-ArgumentList <Args>]
Invoke-Command -Session <Session> -ScriptBlock { <Command> }
```
