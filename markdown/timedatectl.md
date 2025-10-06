# `timedatectl` Command Overview

`timedatectl` is a command-line utility in Linux for querying and changing the system clock and its settings. It can manage time zones, enable or disable time synchronization, and display the current system time configuration.

## Common Options

| Option                     | Description                                         |
|----------------------------|-----------------------------------------------------|
| `status`                   | Show current system time and related information    |
| `set-time <time>`          | Set the system clock to a specified time            |
| `set-timezone <zone>`      | Change the system's time zone                       |
| `list-timezones`           | List all available time zones                       |
| `set-ntp <boolean>`        | Enable or disable Network Time Protocol (NTP) sync   |

## Usage Examples

### Display Current Time Settings

```bash
timedatectl status
```

### Set the System Time

```bash
timedatectl set-time "2023-10-05 15:30:00"
```

### Change the Time Zone

```bash
timedatectl set-timezone America/New_York
```

### List Available Time Zones

```bash
timedatectl list-timezones
```

### Enable NTP Synchronization

```bash
timedatectl set-ntp true
```

## Cheat Sheet

```plaintext
timedatectl status                 # View current time settings
timedatectl set-time "YYYY-MM-DD HH:MM:SS"  # Set the system time
timedatectl set-timezone <zone>    # Change time zone
timedatectl list-timezones         # Display all time zones
timedatectl set-ntp true|false     # Toggle NTP synchronization
```
