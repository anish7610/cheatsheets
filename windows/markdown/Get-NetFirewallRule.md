## `Get-NetFirewallRule` Command

`Get-NetFirewallRule` is a Windows PowerShell command used to retrieve firewall rules configured on a system. It displays information such as the name, display name, description, and status of firewall rules.

### Common Options

| Option                        | Explanation                                                   |
|-------------------------------|---------------------------------------------------------------|
| `-DisplayName <string>`       | Filters rules by their display name.                          |
| `-Name <string>`              | Filters rules by their name.                                  |
| `-Enabled <True|False>`       | Filters rules based on their enabled state.                   |
| `-Direction <Inbound|Outbound>` | Filters rules by their traffic direction.                 |
| `-Action <Allow|Block|Bypass>` | Filters rules based on the action they perform.             |
| `-Profile <Domain|Private|Public>` | Filters rules by the network profile.                |

### Usage Examples

#### List All Firewall Rules

```powershell
Get-NetFirewallRule
```

#### List Enabled Firewall Rules

```powershell
Get-NetFirewallRule -Enabled True
```

#### List Inbound Rules

```powershell
Get-NetFirewallRule -Direction Inbound
```

#### Filter Rules by Display Name

```powershell
Get-NetFirewallRule -DisplayName "My Firewall Rule"
```

#### List Rules that Allow Traffic

```powershell
Get-NetFirewallRule -Action Allow
```

### Cheat Sheet

```plaintext
# List all rules
Get-NetFirewallRule

# List enabled rules
Get-NetFirewallRule -Enabled True

# List inbound rules
Get-NetFirewallRule -Direction Inbound

# Filter by display name
Get-NetFirewallRule -DisplayName "<name>"

# List rules allowing traffic
Get-NetFirewallRule -Action Allow
```
