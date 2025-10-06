# Remove-Item Command in PowerShell

`Remove-Item` is a PowerShell command used to delete files, directories, and other items. It's similar to the `rm` command in Unix-like systems.

## Common Options

| Option                  | Explanation                                                              |
|-------------------------|--------------------------------------------------------------------------|
| `-Path`                 | Specifies the path to the item(s) to remove.                             |
| `-Recurse`              | Deletes all items in the specified directory and its subdirectories.     |
| `-Force`                | Forces the removal of read-only files or hidden items.                   |
| `-WhatIf`               | Shows what would happen if the command is run without actually executing it.|
| `-Filter`               | Specifies a filter to apply to the path. Can simplify and narrow down results.|
| `-Include`              | Specifies, as a string array, items to include.                          |
| `-Exclude`              | Specifies, as a string array, items to exclude.                          |
| `-Confirm`              | Prompts for confirmation before executing the removal.                   |

## Usage Examples

### Delete a Single File

```powershell
Remove-Item -Path "C:\example\file.txt"
```

### Delete All Files in a Directory

```powershell
Remove-Item -Path "C:\example\*"
```

### Delete a Directory and Its Contents

```powershell
Remove-Item -Path "C:\example\" -Recurse
```

### Forcefully Delete Read-Only Files

```powershell
Remove-Item -Path "C:\example\read-only-file.txt" -Force
```

### Simulate Deletion with `-WhatIf`

```powershell
Remove-Item -Path "C:\example\file.txt" -WhatIf
```

### Delete Specific File Types

```powershell
Remove-Item -Path "C:\example\*" -Include "*.txt" -Recurse
```

### Delete Items Except Some

```powershell
Remove-Item -Path "C:\example\*" -Exclude "important.txt"
```

## Cheat Sheet

```plaintext
# Delete a file
Remove-Item -Path "path\to\file"

# Delete all files in a directory
Remove-Item -Path "path\to\directory\*"

# Recursive directory delete
Remove-Item -Path "path\to\directory" -Recurse

# Force delete (includes read-only)
Remove-Item -Path "path\to\file" -Force

# Dry run
Remove-Item -Path "path\to\file" -WhatIf
```
