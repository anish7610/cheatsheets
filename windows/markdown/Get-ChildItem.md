# `Get-ChildItem` Command

`Get-ChildItem` is a Windows PowerShell cmdlet used to list items (files and directories) in one or more specified locations. It is the PowerShell equivalent of the Unix `ls` command.

## Common Options Table

| Option           | Description                                                   |
|------------------|---------------------------------------------------------------|
| `-Path`          | Specifies the path to the location. Can be a filesystem path or registry path. |
| `-Recurse`       | Includes items in subdirectories.                             |
| `-File`          | Gets only files.                                              |
| `-Directory`     | Gets only directories.                                        |
| `-Filter`        | Filters the results using a wildcard pattern.                 |
| `-Name`          | Displays only the names of the items.                         |
| `-Force`         | Includes hidden and system files in the results.              |
| `-Attributes`    | Filters results based on specified file or directory attributes. |

## Usage Examples

### List all files in a directory
```shell
Get-ChildItem -Path "C:\Users\YourName\Documents"
```

### List all files and directories, including those in subdirectories
```shell
Get-ChildItem -Path "C:\Users\YourName\Documents" -Recurse
```

### List only directories
```shell
Get-ChildItem -Path "C:\Users\YourName\Documents" -Directory
```

### List only files with a specific extension
```shell
Get-ChildItem -Path "C:\Users\YourName\Documents" -Filter "*.txt"
```

### List all items, including hidden files
```shell
Get-ChildItem -Path "C:\Users\YourName\Documents" -Force
```

## Cheat Sheet

```shell
# List all items
gci

# List with recursion
gci -Recurse

# List only files
gci -File

# List only directories
gci -Directory

# List with filter
gci -Filter "*.ext"

# Include hidden/system files
gci -Force
```
