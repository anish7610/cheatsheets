# `Get-Help` Command Overview

The `Get-Help` command in Windows PowerShell provides detailed information about PowerShell cmdlets, functions, workflows, aliases, and scripts. It retrieves documentation, including syntax, parameters, and examples.

## Common Options

| Option            | Explanation                                                |
|-------------------|------------------------------------------------------------|
| `-Name <string>`  | Specifies the cmdlet or function you want help with.       |
| `-Full`           | Displays the full help content of the specified command.   |
| `-Examples`       | Shows only the examples for the specified command.         |
| `-Detailed`       | Provides detailed information including parameters.        |
| `-Online`         | Opens online documentation for the command in a browser.   |

## Usage Examples

### 1. Basic Help for a Command
```powershell
Get-Help Get-Process
```

### 2. Detailed Help for a Command
```powershell
Get-Help Get-Process -Detailed
```

### 3. View Examples Only
```powershell
Get-Help Get-Process -Examples
```

### 4. Access Online Documentation
```powershell
Get-Help Get-Process -Online
```

### 5. Full Details of a Command
```powershell
Get-Help Get-Process -Full
```

## Cheat Sheet

```shell
# Basic help
Get-Help <command>

# Detailed view
Get-Help <command> -Detailed

# Examples only
Get-Help <command> -Examples

# Full help
Get-Help <command> -Full

# Online documentation
Get-Help <command> -Online
```
