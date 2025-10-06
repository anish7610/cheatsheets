# Get-LocalUser Command in Windows

## Description

`Get-LocalUser` is a PowerShell cmdlet used to retrieve information about local user accounts on a Windows system.

## Common Options

| Option                   | Explanation                                         |
|--------------------------|-----------------------------------------------------|
| `-Name <String>`         | Specify the name of the local user to retrieve.     |
| `-SID <SecurityIdentifier>` | Retrieve user details using the Security Identifier (SID). |
| `-PrincipalSource <PrincipalSource>` | Filter results by the account type, such as Local or AD. |

## Usage Examples

### List All Local Users

```powershell
Get-LocalUser
```

### Get Specific User Information

```powershell
Get-LocalUser -Name "Alice"
```

### Filter Users by Principal Source

```powershell
Get-LocalUser | Where-Object { $_.PrincipalSource -eq 'Local' }
```

### Check User Existence

```powershell
Get-LocalUser -Name "Bob" | Select-Object Name, Enabled
```

## Cheat Sheet

```plaintext
Get-LocalUser                # List all local users
Get-LocalUser -Name "User"   # Get info for a specific user
```
