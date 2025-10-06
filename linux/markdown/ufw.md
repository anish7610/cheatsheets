# UFW Command Overview

`ufw` (Uncomplicated Firewall) is a user-friendly front-end for managing iptables firewall rules. It simplifies the process of setting up and configuring a firewall in Linux systems.

## Common Options

| Option          | Description                                             |
|-----------------|---------------------------------------------------------|
| `enable`        | Activates the firewall.                                 |
| `disable`       | Deactivates the firewall.                               |
| `status`        | Displays the current status of the firewall.            |
| `allow <service/port>`  | Permits incoming traffic on a specified port or service. |
| `deny <service/port>`   | Blocks incoming traffic on a specified port or service.  |
| `delete <rule>` | Removes a specified rule.                               |
| `reset`         | Resets the firewall to its default state, removing all rules. |
| `default allow|deny` | Sets default policy for incoming connections to allow or deny. |

## Usage Examples

```bash
# Enable the firewall
sudo ufw enable

# Disable the firewall
sudo ufw disable

# Allow incoming traffic on port 22 (SSH)
sudo ufw allow 22

# Deny incoming traffic on port 80 (HTTP)
sudo ufw deny 80

# Check the current firewall status and rules
sudo ufw status

# Remove a specific rule allowing SSH
sudo ufw delete allow 22

# Set the default policy to deny all incoming connections
sudo ufw default deny
```

## Cheat Sheet

```plaintext
sudo ufw enable                # Enable firewall
sudo ufw disable               # Disable firewall
sudo ufw status                # Check firewall status
sudo ufw allow <port/service>  # Allow traffic
sudo ufw deny <port/service>   # Deny traffic
sudo ufw delete <rule>         # Remove rule
sudo ufw default allow|deny    # Set default policy
```
