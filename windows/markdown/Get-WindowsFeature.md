# Get-WindowsFeature

`Get-WindowsFeature` is a Windows PowerShell command used to display information about roles and features installed on a Windows server. It helps administrators manage and verify installed components efficiently.

## Common Options

| Option                  | Explanation                                                 |
|-------------------------|-------------------------------------------------------------|
| `-Name <string>`        | Displays information for a specific role or feature by name.|
| `-ComputerName <string>`| Queries features on a remote computer.                      |
| `-Credential <pscredential>`| Specifies user credentials for remote access.              |
| `-LogPath <string>`     | Specifies a log file path for output.                       |

## Examples

### List All Installed Features
```powershell
Get-WindowsFeature
```

### Check a Specific Feature
```powershell
Get-WindowsFeature -Name Web-Server
```

### List Features on a Remote Computer
```powershell
Get-WindowsFeature -ComputerName Server01
```

### Use Credentials for Remote Query
```powershell
$cred = Get-Credential
Get-WindowsFeature -ComputerName Server01 -Credential $cred
```

## Cheat Sheet

```plaintext
# List all features
Get-WindowsFeature

# Check a specific feature
Get-WindowsFeature -Name <feature-name>

# Query remote server
Get-WindowsFeature -ComputerName <server-name>

# Use credentials for remote
$cred = Get-Credential
Get-WindowsFeature -ComputerName <server-name> -Credential $cred
```
