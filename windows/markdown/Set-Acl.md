# Set-Acl Command Overview

`Set-Acl` is a Windows PowerShell command used to modify the Access Control List (ACL) of files and folders, controlling the permissions for system objects.

## Common Options

| Option                  | Description                                              |
|-------------------------|----------------------------------------------------------|
| `-Path`                 | Specifies the path to the file or directory.             |
| `-AclObject`            | Specifies the ACL object to apply to the item.           |
| `-InputObject`          | Accepts pipeline input of the path to the ACL item.      |

## Usage Examples

### Example 1: Set Permissions on a File
```powershell
$acl = Get-Acl "C:\example\file.txt"
$permission = "DOMAIN\User", "FullControl", "Allow"
$accessRule = New-Object System.Security.AccessControl.FileSystemAccessRule $permission
$acl.SetAccessRule($accessRule)
Set-Acl -Path "C:\example\file.txt" -AclObject $acl
```

### Example 2: Pipeline Usage for a Directory
```powershell
$acl = Get-Acl "C:\example\"
$permission = "DOMAIN\User", "Read", "Allow"
$accessRule = New-Object System.Security.AccessControl.FileSystemAccessRule $permission
$acl.AddAccessRule($accessRule)
Get-ChildItem "C:\example\" | Set-Acl -AclObject $acl
```

### Example 3: Copy ACL from One File to Another
```powershell
$sourceAcl = Get-Acl "C:\source\file.txt"
Set-Acl -Path "C:\destination\file.txt" -AclObject $sourceAcl
```

## Cheat Sheet

```plaintext
Get-Acl <Path>          # Retrieve ACL of file or directory
Set-Acl -Path <Path> -AclObject <Acl>   # Apply ACL to a file or directory
New-Object System.Security.AccessControl.FileSystemAccessRule <User>, <Rights>, <Type>   # Create a new access rule
```
