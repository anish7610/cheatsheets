# Get-Acl Command in PowerShell

`Get-Acl` is a PowerShell cmdlet used to retrieve the security descriptor, which includes access control lists (ACLs), for a specified item such as a file, folder, or registry key. This helps manage permissions efficiently.

## Common Options

| Option                  | Description                                               |
|-------------------------|-----------------------------------------------------------|
| `-Path`                 | Specifies the path to the item (file, folder, etc.).      |
| `-LiteralPath`          | Specifies an exact path without wildcard expansion.       |
| `-Filter`               | String to filter paths when retrieving ACLs.              |
| `-Audit`                | Retrieves only the audit rules of the item.               |
| `-Access`               | Retrieves only the access rules of the item.              |

## Usage Examples

### Retrieve ACL for a File
```powershell
Get-Acl -Path "C:\example\file.txt"
```

### Retrieve ACL with Access Rules Only
```powershell
Get-Acl -Path "C:\example\file.txt" -Access
```

### Retrieve ACL for a Directory
```powershell
Get-Acl -Path "C:\example\"
```

### Retrieve ACL Using Literal Path
```powershell
Get-Acl -LiteralPath "C:\example\[special]file.txt"
```

## Cheat Sheet

```shell
Get-Acl -Path <path>          # Retrieve ACL for a given path
Get-Acl -Access               # Get access rules only
Get-Acl -Audit                # Get audit rules only
Get-Acl -LiteralPath <path>   # Use without expanding wildcards
```
