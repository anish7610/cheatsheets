# Get-Volume Command

`Get-Volume` is a Windows PowerShell command used to retrieve information about volumes on a system. It displays details such as volume size, file system, and drive letter.

## Common Options

| Option              | Explanation                                               |
|---------------------|-----------------------------------------------------------|
| `-DriveLetter <char>` | Filters the output by specifying the drive letter.       |
| `-FileSystem <name>`  | Filters volumes by the file system type (e.g., NTFS).    |
| `-CimSession <session>` | Runs the command in a specified remote session.        |
| `-Detailed`           | Provides expanded output including additional details.   |

## Usage Examples

### Example 1: Retrieve all volumes
```powershell
Get-Volume
```

### Example 2: Get volumes by drive letter
```powershell
Get-Volume -DriveLetter C
```

### Example 3: List volumes with NTFS file system
```powershell
Get-Volume -FileSystem NTFS
```

### Example 4: Get detailed information on all volumes
```powershell
Get-Volume -Detailed
```

## Cheat Sheet

```plaintext
Get-Volume                  # List all volumes
Get-Volume -DriveLetter C   # Filter by drive letter
Get-Volume -FileSystem NTFS # Filter by file system type
Get-Volume -Detailed        # Detailed information
```
