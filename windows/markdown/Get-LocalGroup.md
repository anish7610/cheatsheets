# `Get-LocalGroup` Command in Windows

## Description

`Get-LocalGroup` is a PowerShell command used to retrieve information about local groups on a Windows system. It provides details about the groups available on the local computer, such as their names and descriptions.

## Common Options

| Option          | Description                                              |
|-----------------|----------------------------------------------------------|
| `-Name <String>`| Filter and retrieve a specific local group by name.      |
| `-Sid <String>` | Retrieve a local group using its Security Identifier.    |

## Usage Examples

### List All Local Groups

```powershell
Get-LocalGroup
```

### Get Information About a Specific Group

```powershell
Get-LocalGroup -Name "Administrators"
```

### Retrieve a Group by SID

```powershell
Get-LocalGroup -Sid "S-1-5-32-544"
```

## Cheat Sheet

```plaintext
# List all groups
Get-LocalGroup

# Get specific group by name
Get-LocalGroup -Name "<GroupName>"

# Get group by SID
Get-LocalGroup -Sid "<SID>"
```
