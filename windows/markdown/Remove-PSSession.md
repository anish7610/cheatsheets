### Description

`Remove-PSSession` is a Windows PowerShell command used to close and remove one or more PowerShell sessions (PSSessions). This helps manage system resources and ensures no lingering open sessions.

### Common Options

| Option       | Explanation                                          |
|--------------|------------------------------------------------------|
| `-Id`        | Specifies the IDs of the PSSession objects to remove.|
| `-Session`   | Directly specifies the PSSession objects to remove.  |
| `-Name`      | Specifies the names of the PSSession objects to remove. |
| `-InstanceId`| Specifies the instance IDs of the PSSessions to remove. |
| `-ThrottleLimit` | Sets a limit on the number of concurrent operations. |

### Usage Examples

#### Remove a Session by ID
```powershell
Remove-PSSession -Id 1
```

#### Remove Multiple Sessions by ID
```powershell
Remove-PSSession -Id 1,2,3
```

#### Remove a Session by Name
```powershell
Remove-PSSession -Name "SessionName"
```

#### Remove a Session Using a Session Object
```powershell
$session = New-PSSession -ComputerName "Server01"
Remove-PSSession -Session $session
```

#### Remove All Open Sessions
```powershell
Get-PSSession | Remove-PSSession
```

### Cheat Sheet

```plaintext
# Remove session by ID(s)
Remove-PSSession -Id <session_id>

# Remove session by name
Remove-PSSession -Name "<session_name>"

# Remove session by session object
Remove-PSSession -Session $session

# Remove all sessions
Get-PSSession | Remove-PSSession
```
