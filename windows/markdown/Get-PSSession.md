# Get-PSSession Command in Windows

`Get-PSSession` is a PowerShell command used to retrieve information about existing PowerShell sessions (PSSessions) on local and remote computers.

## Common Options

| Option               | Explanation                                                                            |
|----------------------|----------------------------------------------------------------------------------------|
| `-ComputerName`      | Specifies the name of the computer to check for PSSessions.                            |
| `-Name`              | Filters the sessions by name.                                                          |
| `-InstanceId`        | Filters the sessions by their instance IDs.                                            |
| `-Id`                | Filters the sessions by their session IDs.                                             |
| `-ThrottleLimit`     | Limits the number of concurrent operations.                                             |

## Usage Examples

### List All Local PSSessions
```powershell
Get-PSSession
```

### List All PSSessions on a Remote Computer
```powershell
Get-PSSession -ComputerName "RemotePC"
```

### Filter Sessions by Name
```powershell
Get-PSSession -Name "MySessionName"
```

### Filter Sessions by Instance ID
```powershell
$instanceId = [guid]"4f24e8d1-2f5f-4b0b-bb8a-e4f0d78e9f8d"
Get-PSSession -InstanceId $instanceId
```

### Limit Concurrent Operations
```powershell
Get-PSSession -ComputerName "RemotePC" -ThrottleLimit 5
```

## Cheat Sheet

- **List Local Sessions**: `Get-PSSession`
- **Remote Sessions**: `Get-PSSession -ComputerName "RemotePC"`
- **Filter by Name**: `Get-PSSession -Name "SessionName"`
- **Specific Instance**: `Get-PSSession -InstanceId [guid]`
- **Throttle Operations**: `-ThrottleLimit [number]`
