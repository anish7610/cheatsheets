# `Get-SqlInstance` Command

`Get-SqlInstance` is a PowerShell command used to discover SQL Server instances on the network or locally. It helps administrators quickly find available SQL Server instances without needing to manually check each server.

## Common Options

| Option                | Description                                                                     |
|-----------------------|---------------------------------------------------------------------------------|
| `-ServerName`         | Specifies the name of the server to search for SQL instances.                   |
| `-Credential`         | Specifies the user credentials to access the remote server.                     |
| `-DiscoverySource`    | Allows you to set the source of discovery (`Network`, `LocalRegistry`, `SSDT`). |
| `-EnableException`    | Indicates whether exceptions should be displayed.                               |

## Usage Examples

### Discover All SQL Instances on the Local Network

```powershell
Get-SqlInstance -DiscoverySource Network
```

### Find SQL Instances on a Specific Server

```powershell
Get-SqlInstance -ServerName "MyServer"
```

### Discover SQL Instances with Specific Credentials

```powershell
$credential = Get-Credential
Get-SqlInstance -ServerName "MyServer" -Credential $credential
```

### Use Local Registry for Discovery

```powershell
Get-SqlInstance -DiscoverySource LocalRegistry
```

## Cheat Sheet

```plaintext
# Find SQL instances on the network
Get-SqlInstance -DiscoverySource Network

# Find SQL instances on a specific server
Get-SqlInstance -ServerName "ServerNameHere"

# Use specific credentials
Get-SqlInstance -ServerName "MyServer" -Credential (Get-Credential)

# Discover using local registry
Get-SqlInstance -DiscoverySource LocalRegistry
```
