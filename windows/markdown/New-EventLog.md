# `New-EventLog` Command

`New-EventLog` is a PowerShell command used to create a new event log on a local or remote computer and optionally define new event sources.

## Common Options

| Option                | Description                                                           |
|-----------------------|-----------------------------------------------------------------------|
| `-LogName`            | Specifies the name of the new event log.                              |
| `-Source`             | Defines one or more new sources to be associated with the event log.  |
| `-ComputerName`       | Specifies the target computer for the event log creation.             |
| `-MessageResourceFile`| Defines a message resource file for event descriptions.               |
| `-CategoryResourceFile`| Specifies a category resource file for the event log.               |

## Usage Examples

### Example 1: Create a New Event Log
```powershell
New-EventLog -LogName "ApplicationLog" -Source "MyApp"
```
Creates a new event log named "ApplicationLog" with a source "MyApp".

### Example 2: Create an Event Log on a Remote Computer
```powershell
New-EventLog -LogName "RemoteAppLog" -Source "RemoteApp" -ComputerName "Server01"
```
Creates "RemoteAppLog" on "Server01" with source "RemoteApp".

### Example 3: Define Resource Files
```powershell
New-EventLog -LogName "AppLog" -Source "App" -MessageResourceFile "C:\Logs\MsgResource.dll" -CategoryResourceFile "C:\Logs\CatResource.dll"
```
Associates resource files with the "AppLog" event log.

## Cheat Sheet

```plaintext
# Create an event log with a source
New-EventLog -LogName "<LogName>" -Source "<Source>"

# Create an event log on a remote computer
New-EventLog -LogName "<LogName>" -Source "<Source>" -ComputerName "<ComputerName>"

# Define message and category resource files
New-EventLog -LogName "<LogName>" -Source "<Source>" -MessageResourceFile "<PathToMessageResource>" -CategoryResourceFile "<PathToCategoryResource>"
```
