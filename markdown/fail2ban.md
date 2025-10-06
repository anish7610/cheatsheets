## Fail2ban Command Overview

`fail2ban` is a security utility that protects Linux systems from brute-force attacks. It scans log files for predefined patterns and bans IPs using firewall rules.

## Common Options

| Option              | Description                                                                  |
|---------------------|------------------------------------------------------------------------------|
| `fail2ban-client`   | Main command to interact with Fail2ban.                                      |
| `start`             | Starts the Fail2ban service.                                                 |
| `stop`              | Stops the Fail2ban service.                                                  |
| `restart`           | Restarts the Fail2ban service.                                               |
| `status`            | Shows the status of the Fail2ban service and all active jails.               |
| `add <JAIL>`        | Enables a specific jail.                                                     |
| `del <JAIL>`        | Disables a specific jail.                                                    |
| `status <JAIL>`     | Shows the status and banned IPs for a specific jail.                         |
| `set <JAIL> banip`  | Manually bans an IP on a specific jail.                                      |
| `unbanip <JAIL>`    | Removes the ban for a specific IP.                                           |

## Usage Examples

### Start Fail2ban Service
```bash
sudo fail2ban-client start
```

### Check the Status of All Jails
```bash
sudo fail2ban-client status
```

### Check the Status of a Specific Jail
```bash
sudo fail2ban-client status sshd
```

### Manually Ban an IP in a Jail
```bash
sudo fail2ban-client set sshd banip 192.168.1.100
```

### Unban an IP in a Jail
```bash
sudo fail2ban-client set sshd unbanip 192.168.1.100
```

## Cheat Sheet

```plaintext
Start: sudo fail2ban-client start
Stop: sudo fail2ban-client stop
Status: sudo fail2ban-client status
Jail Status: sudo fail2ban-client status <JAIL>
Ban IP: sudo fail2ban-client set <JAIL> banip <IP>
Unban IP: sudo fail2ban-client set <JAIL> unbanip <IP>
```
