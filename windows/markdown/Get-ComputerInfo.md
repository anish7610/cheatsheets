# `Get-ComputerInfo` Command

`Get-ComputerInfo` is a PowerShell command in Windows used to retrieve detailed information about the local computer system.

## Common Options

| Option                  | Explanation                                        |
|-------------------------|----------------------------------------------------|
| `-Property`             | Specifies which property or properties to display. |
| `-ErrorAction`          | Defines action to take if command encounters an error. |
| `-IncludeUserName`      | Includes the username of the currently logged-on user. |

## Usage Examples

### Example 1: Retrieve Basic System Information
```powershell
Get-ComputerInfo
```
This outputs complete system information including OS, BIOS, CPU details, etc.

### Example 2: Retrieve Specific Properties
```powershell
Get-ComputerInfo -Property "CsName", "WindowsVersion", "CsProcessors"
```
This displays system name, Windows version, and processor details.

### Example 3: Handle Errors Gracefully
```powershell
Get-ComputerInfo -ErrorAction SilentlyContinue
```
Suppresses error messages if the command fails.

## Cheat Sheet

```plaintext
# Basic info
Get-ComputerInfo

# Select specific properties
Get-ComputerInfo -Property "Property1", "Property2"

# Error handling
Get-ComputerInfo -ErrorAction <Action>
```
