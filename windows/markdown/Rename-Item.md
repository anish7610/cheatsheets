# Rename-Item Command

`Rename-Item` is a PowerShell cmdlet used to rename files, directories, and other objects.

## Common Options

| Option            | Description                                      |
|-------------------|--------------------------------------------------|
| `-Path`           | Specifies the path to the item to be renamed.    |
| `-NewName`        | Specifies the new name for the item.             |
| `-Force`          | Forces the command to execute without asking.    |
| `-WhatIf`         | Shows what would happen if the command runs.     |
| `-Verbose`        | Provides detailed operation information.         |
| `-Confirm`        | Prompts for confirmation before proceeding.      |

## Usage Examples

### Rename a Single File

```powershell
Rename-Item -Path "C:\Files\oldfile.txt" -NewName "newfile.txt"
```

### Rename a Directory

```powershell
Rename-Item -Path "C:\Files\OldFolder" -NewName "NewFolder"
```

### Rename Multiple Files Using a Loop

```powershell
Get-ChildItem -Path "C:\Files\" -Filter "*.txt" | ForEach-Object {
    Rename-Item -Path $_.FullName -NewName ("newname_" + $_.Name)
}
```

### Force Rename Without Prompt

```powershell
Rename-Item -Path "C:\Files\readonlyfile.txt" -NewName "newfile.txt" -Force
```

### Simulate Rename Without Executing

```powershell
Rename-Item -Path "C:\Files\oldfile.txt" -NewName "newfile.txt" -WhatIf
```

## Cheat Sheet

```plaintext
Rename-Item -Path <old_path> -NewName <new_name>
-Force          # Execute without prompt
-WhatIf         # Show what would happen
-Verbose        # Detailed output
-Confirm        # Prompt for confirmation
```
