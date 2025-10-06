# `firewalld` Command Overview

`firewalld` is a dynamic firewall management tool for Linux, providing a firewall with support for network/firewall zones. It allows for the easy configuration of firewall rules without requiring a complete reload.

## Common Options

| Option                | Explanation                                                |
|-----------------------|------------------------------------------------------------|
| `--get-zones`         | List all available zones.                                  |
| `--get-active-zones`  | List zones with active connections.                        |
| `--list-all`          | Display comprehensive information on active zones.         |
| `--add-service=<svc>` | Add a predefined service to a zone.                        |
| `--remove-service=<svc>` | Remove a predefined service from a zone.                |
| `--zone=<zone>`       | Specify the zone to apply other options to.                |
| `--reload`            | Reload `firewalld` rules and configurations.               |
| `--permanent`         | Make changes persistent across reboots.                    |

## Usage Examples

### List All Zones
```bash
firewall-cmd --get-zones
```

### Display Active Zones
```bash
firewall-cmd --get-active-zones
```

### List All Rules in a Zone
```bash
firewall-cmd --zone=public --list-all
```

### Add a Service to a Zone
```bash
firewall-cmd --zone=public --add-service=http
```

### Remove a Service from a Zone
```bash
firewall-cmd --zone=public --remove-service=http
```

### Make Changes Permanent
```bash
firewall-cmd --zone=public --add-service=https --permanent
```

### Reload Firewall to Apply Changes
```bash
firewall-cmd --reload
```

## Cheat Sheet

```plaintext
- List zones: firewall-cmd --get-zones
- Check active zones: firewall-cmd --get-active-zones
- Check zone rules: firewall-cmd --zone=<zone> --list-all
- Add service: firewall-cmd --zone=<zone> --add-service=<svc> [--permanent]
- Remove service: firewall-cmd --zone=<zone> --remove-service=<svc> [--permanent]
- Reload changes: firewall-cmd --reload
```
