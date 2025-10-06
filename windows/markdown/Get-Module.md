# Get-Module Command in Windows

`Get-Module` is a PowerShell command used to retrieve information about the modules imported into the current session or available on the system.

## Common Options

| Option            | Description                                                       |
|-------------------|-------------------------------------------------------------------|
| `-ListAvailable`  | Lists all modules installed on the system, not just imported ones.|
| `-Name <string>`  | Specifies the name of the module to display information about.    |
| `-All`            | Retrieves all the module versions available on the system.        |
| `-FullyQualifiedName` | Retrieves modules using their full name.                     |

## Usage Examples

### List All Imported Modules
```powershell
Get-Module
```

### List All Available Modules
```powershell
Get-Module -ListAvailable
```

### Get Information About a Specific Module
```powershell
Get-Module -Name <ModuleName>
```

### List All Versions of a Module
```powershell
Get-Module -Name <ModuleName> -All
```

## Cheat Sheet

```plaintext
# List imported modules
Get-Module

# List all available modules
Get-Module -ListAvailable

# Get details of a specific module
Get-Module -Name <ModuleName>

# List all versions of a specific module
Get-Module -Name <ModuleName> -All
```
