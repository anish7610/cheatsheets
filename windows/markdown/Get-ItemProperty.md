## Description

The `Get-ItemProperty` command in Windows PowerShell retrieves the properties of a specified item, such as a file, registry key, or any other item. It is especially useful for extracting metadata or attributes.

## Common Options

| Option          | Explanation                                      |
|-----------------|--------------------------------------------------|
| `-Path`         | Specifies the path of the item to get properties from. |
| `-Name`         | Retrieves specific properties by name.           |
| `-Exclude`      | Excludes specified properties from the results.  |
| `-Include`      | Limits retrieval to specified properties.        |
| `-LiteralPath`  | Specifies the path exactly as typed (no wildcard expansion). |

## Usage Examples

### Retrieve File Properties

```powershell
Get-ItemProperty -Path "C:\path\to\file.txt"
```

### Get Specific Property of a File

```powershell
Get-ItemProperty -Path "C:\path\to\file.txt" -Name "LastWriteTime"
```

### Retrieve Registry Key Properties

```powershell
Get-ItemProperty -Path "HKLM:\Software\Microsoft\Windows"
```

### Exclude Certain Properties

```powershell
Get-ItemProperty -Path "C:\path\to\file.txt" -Exclude "LastAccessTime"
```

## Cheat Sheet

```plaintext
# Get all properties of a file
Get-ItemProperty -Path "<file_path>"

# Get specific property of a file
Get-ItemProperty -Path "<file_path>" -Name "<property_name>"

# Get properties of a registry key
Get-ItemProperty -Path "<registry_path>"

# Exclude specific properties
Get-ItemProperty -Path "<file_path>" -Exclude "<property_name>"
```
