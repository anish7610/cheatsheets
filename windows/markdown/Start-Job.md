# Start-Job Command in PowerShell

## Description

`Start-Job` is a PowerShell command used to run scripts or commands in the background, allowing you to continue working in the session without waiting for the command to complete.

## Common Options

| Option               | Explanation                                                   |
|----------------------|---------------------------------------------------------------|
| `-ScriptBlock`       | Specifies the command or script to run in the background.     |
| `-FilePath`          | Runs a script from a specified file path.                     |
| `-Name`              | Assigns a name to the job for easier identification.          |
| `-ArgumentList`      | Passes arguments to the script or command.                    |
| `-Credential`        | Specifies a user credential for running the job.              |
| `-InitializationScript` | Runs a script block before the job starts.                 |

## Examples

### Example 1: Running a Background Job

```powershell
Start-Job -ScriptBlock { Get-Process }
```

### Example 2: Running a Script from a File

```powershell
Start-Job -FilePath "C:\Scripts\MyScript.ps1"
```

### Example 3: Running a Job with Arguments

```powershell
Start-Job -ScriptBlock {
    param($a, $b)
    $a + $b
} -ArgumentList 5, 10
```

### Example 4: Assigning a Name to a Job

```powershell
Start-Job -ScriptBlock { Get-Date } -Name "DateJob"
```

### Example 5: Using User Credentials

```powershell
Start-Job -ScriptBlock { Get-Process } -Credential (Get-Credential)
```

## Cheat Sheet

```plaintext
Start-Job -ScriptBlock { <cmd> } [-ArgumentList <args>] [-Name <name>]
Start-Job -FilePath "<path>" [-ArgumentList <args>] [-Name <name>]
```
