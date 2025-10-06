# Get-WebAppPool Command Overview

The `Get-WebAppPool` command in Windows is used to retrieve information about application pools in Internet Information Services (IIS). It's part of the WebAdministration module.

## Common Options

| Option             | Description                                         |
|--------------------|-----------------------------------------------------|
| `-Name <string>`   | Specifies the name of the application pool to retrieve. |
| `-PSPath <string>` | Specifies the path to the IIS configuration to query. |

## Usage Examples

### List All Application Pools

```powershell
Get-WebAppPool
```

### Get a Specific Application Pool

```powershell
Get-WebAppPool -Name "DefaultAppPool"
```

### Get Application Pool with Specific PSPath

```powershell
Get-WebAppPool -PSPath "IIS:\AppPools"
```

## Cheat Sheet

```plaintext
# List all app pools
Get-WebAppPool

# Get a specific app pool by name
Get-WebAppPool -Name "AppPoolName"

# Get app pool using path
Get-WebAppPool -PSPath "IIS:\AppPools"
```
