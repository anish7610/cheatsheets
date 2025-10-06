# `Set-ItemProperty` Command Overview

The `Set-ItemProperty` cmdlet in Windows PowerShell is used to modify property values of items, typically files or registry keys. It provides a straightforward way to change settings or attributes of specific items in the file system or registry.

## Common Options

| Option               | Description                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| `-Path`              | Specifies the path to the item whose properties you want to modify.         |
| `-Name`              | Specifies the name of the property you want to change.                       |
| `-Value`             | Specifies the new value for the property.                                    |
| `-LiteralPath`       | Specifies the path to the item with no wildcard characters or interpretation.|
| `-Credential`        | Specifies a user account that has permission to perform this action.         |
| `-PassThru`          | Outputs the object with the modified property to the pipeline.               |
| `-Force`             | Forces the command to execute, even for restricted items.                   |

## Usage Examples

### Modify a File Property

```powershell
Set-ItemProperty -Path "C:\Example\File.txt" -Name IsReadOnly -Value $false
```
This command changes the `IsReadOnly` property of `File.txt` to `False`.

### Change a Registry Key Value

```powershell
Set-ItemProperty -Path "HKCU:\Software\MyApp" -Name "Setting" -Value "NewValue"
```
This modifies the `Setting` property of the `MyApp` registry key to `NewValue`.

### Using Literal Path

```powershell
Set-ItemProperty -LiteralPath "C:\Path[With]Special*Chars.txt" -Name ReadOnly -Value $true
```
This sets the `ReadOnly` property of a file with special characters in its name to `True`.

## Cheat Sheet

```plaintext
Set-ItemProperty -Path <path> -Name <property_name> -Value <new_value>
Set-ItemProperty -Path <path> -Name <property> -Value <value> -PassThru
Set-ItemProperty -Path <path> -Name <property> -Value <value> -Force
```
