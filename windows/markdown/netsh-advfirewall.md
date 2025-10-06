# `netsh advfirewall`

`netsh advfirewall` is a command-line tool in Windows used for configuring and managing the Windows Firewall with Advanced Security. It allows for the detailed control and customization of firewall settings.

## Common Options

| Option                          | Explanation                                                       |
|---------------------------------|-------------------------------------------------------------------|
| `set allprofiles state`         | Enable or disable the firewall for all profiles.                  |
| `set currentprofile state`      | Enable or disable the firewall for the current profile.           |
| `set domainprofile state`       | Configure the firewall for the domain profile.                    |
| `set privateprofile state`      | Configure the firewall for the private profile.                   |
| `set publicprofile state`       | Configure the firewall for the public profile.                    |
| `add rule`                      | Add a new firewall rule.                                          |
| `delete rule`                   | Delete an existing firewall rule.                                 |
| `show allprofiles`              | Display the current firewall settings for all profiles.           |
| `show currentprofile`           | Display the current profile’s firewall settings.                  |
| `set rule`                      | Modify an existing firewall rule.                                 |

## Usage Examples

### Enable Firewall for All Profiles
```bash
netsh advfirewall set allprofiles state on
```

### Disable Firewall for All Profiles
```bash
netsh advfirewall set allprofiles state off
```

### Add a Firewall Rule to Allow Inbound HTTP Traffic
```bash
netsh advfirewall firewall add rule name="AllowHTTP" protocol=TCP dir=in localport=80 action=allow
```

### Delete a Firewall Rule by Name
```bash
netsh advfirewall firewall delete rule name="AllowHTTP"
```

### Show Firewall Settings for Current Profile
```bash
netsh advfirewall show currentprofile
```

## Cheat Sheet

```markdown
Enable Firewall:
netsh advfirewall set allprofiles state on

Disable Firewall:
netsh advfirewall set allprofiles state off

Add Rule (Allow HTTP):
netsh advfirewall firewall add rule name="AllowHTTP" protocol=TCP dir=in localport=80 action=allow

Delete Rule:
netsh advfirewall firewall delete rule name="AllowHTTP"

Show Current Profile Settings:
netsh advfirewall show currentprofile
```
