# Get-Command: Quick Guide

`Get-Command` is a Windows PowerShell cmdlet used to retrieve all the commands available, including cmdlets, functions, aliases, and executables. It helps users discover and explore what commands they can use.

## Common Options

| Option            | Description                                                  |
|-------------------|--------------------------------------------------------------|
| `-Name`           | Specifies the name of the command to retrieve.               |
| `-CommandType`    | Filters results by command type (e.g., cmdlet, function).    |
| `-Module`         | Limits results to commands in a specific module.             |
| `-Syntax`         | Displays the syntax of one or more commands.                 |
| `-Noun`           | Filters results by the noun part of cmdlet names.            |
| `-Verb`           | Filters results by the verb part of cmdlet names.            |

## Usage Examples

### List All Cmdlets
```powershell
Get-Command -CommandType Cmdlet
```

### Find Commands by Name
```powershell
Get-Command -Name *Service*
```

### Display Syntax for Specific Command
```powershell
Get-Command -Name Get-Process -Syntax
```

### List Commands in a Module
```powershell
Get-Command -Module Microsoft.PowerShell.Management
```

### Find Commands by Verb
```powershell
Get-Command -Verb Get
```

## Cheat Sheet

```plaintext
Get-Command -Name <Pattern>
Get-Command -CommandType <Type>
Get-Command -Module <ModuleName>
Get-Command -Syntax
Get-Command -Noun <Noun>
Get-Command -Verb <Verb>
```
