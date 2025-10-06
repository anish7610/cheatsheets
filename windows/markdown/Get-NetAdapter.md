# Get-NetAdapter Command

`Get-NetAdapter` is a PowerShell command used to retrieve the network adapter configuration of a Windows system. It provides detailed information about network interfaces, including their states, properties, and statistics.

## Common Options

| Option                  | Explanation                                                     |
|-------------------------|-----------------------------------------------------------------|
| `-Name <string[]>`      | Specifies the name of the network adapter(s) to retrieve.       |
| `-InterfaceDescription` | Filters network adapters by their interface description.        |
| `-Physical`             | Shows only physical network adapters, excluding virtual ones.   |
| `-IncludeHidden`        | Includes hidden network adapters in the displayed result.       |
| `-CimSession`           | Allows the command to be run on a remote computer.              |

## Usage Examples

### List All Network Adapters

```powershell
Get-NetAdapter
```

### Filter by Adapter Name

```powershell
Get-NetAdapter -Name "Ethernet"
```

### Display Only Physical Adapters

```powershell
Get-NetAdapter -Physical
```

### Include Hidden Adapters

```powershell
Get-NetAdapter -IncludeHidden
```

### Run on a Remote Machine

```powershell
Get-NetAdapter -CimSession Server01
```

## Cheat Sheet

```plaintext
# List all adapters
Get-NetAdapter

# Filter by name
Get-NetAdapter -Name "Ethernet"

# Only physical adapters
Get-NetAdapter -Physical

# Include hidden adapters
Get-NetAdapter -IncludeHidden

# Remote session
Get-NetAdapter -CimSession <RemoteComputer>
```
