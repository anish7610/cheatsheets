# Get-NetFirewallProfile Command

The `Get-NetFirewallProfile` command in Windows is part of the PowerShell `NetSecurity` module. It retrieves configuration details of firewall profiles: Domain, Private, and Public.

## Common Options

| Option                    | Explanation                                         |
|---------------------------|-----------------------------------------------------|
| `-Profile <string[]>`     | Specifies one or more profiles (Domain, Private, Public). |
| `-CimSession <CimSession>`| Runs the command on a remote session.               |
| `-PolicyStore <string>`   | Defines the policy store to pull from (e.g., ActiveStore). |

## Usage Examples

### Retrieve All Firewall Profiles

```powershell
Get-NetFirewallProfile
```

### Retrieve a Specific Profile (e.g., Domain)

```powershell
Get-NetFirewallProfile -Profile Domain
```

### Retrieve Firewall Profiles on a Remote Computer

```powershell
$session = New-CimSession -ComputerName "RemotePC"
Get-NetFirewallProfile -CimSession $session
```

## Cheat Sheet

```plaintext
# Get all firewall profiles
Get-NetFirewallProfile

# Get specific profile
Get-NetFirewallProfile -Profile Domain

# Remote computer profile
Get-NetFirewallProfile -CimSession (New-CimSession -ComputerName "RemotePC")
```
