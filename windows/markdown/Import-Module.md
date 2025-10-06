# `Import-Module` Command Overview

`Import-Module` is a PowerShell command used to load modules into the current session, giving you access to their cmdlets, functions, aliases, and resources.

## Common Options

| Option           | Description                                                                                  |
|------------------|----------------------------------------------------------------------------------------------|
| `-Name`          | Specifies the name of the module to import.                                                  |
| `-Force`         | Forces the module to import, overwriting any existing imported modules with the same name.   |
| `-Scope`         | Specifies the scope in which the module is imported (e.g., Global, Local).                   |
| `-PassThru`      | Returns a module object that represents the modules being imported.                          |
| `-DisableNameChecking` | Suppresses warning messages that might occur if the module name contains invalid characters. |

## Usage Examples

### Import a Module by Name

```powershell
Import-Module -Name PSReadLine
```

### Force Import a Module

```powershell
Import-Module -Name MyCustomModule -Force
```

### Import a Module and Return the Object

```powershell
$moduleObj = Import-Module -Name MyModule -PassThru
```

### Import a Module with a Specific Scope

```powershell
Import-Module -Name NetworkModule -Scope Global
```

## Cheat Sheet

```plaintext
Import-Module -Name <moduleName>
Import-Module -Name <moduleName> -Force
Import-Module -Name <moduleName> -PassThru
Import-Module -Name <moduleName> -Scope <ScopeType>
```
