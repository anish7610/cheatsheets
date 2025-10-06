# Understanding the `last` Command in Linux

The `last` command in Linux is used to display a list of the most recent logins, reboots, and shutdowns by reading the `/var/log/wtmp` file.

## Common Options

| Option    | Description                                              |
|-----------|----------------------------------------------------------|
| `-n N`    | Show the last N lines (entries).                         |
| `-a`      | Display the hostname in the last column.                 |
| `-d`      | Translate IP addresses to hostnames.                     |
| `-F`      | Show complete login and logout times and dates.          |
| `-x`      | Show system shutdown, runlevel changes, and boots.       |

## Usage Examples

### Show Last 5 Logins
```bash
last -n 5
```

### Display Hostnames in Last Column
```bash
last -a
```

### Translate IP to Hostnames
```bash
last -d
```

### Show Complete Dates for Logins
```bash
last -F
```

### Display Reboots and Shutdowns
```bash
last -x
```

## Cheat Sheet

```plaintext
last         # Show login history
last -n 5    # Show last 5 logins
last -a      # Hostname in last column
last -d      # IP addresses to hostnames
last -F      # Full date and time
last -x      # Show boots, shutdowns, runlevels
```
