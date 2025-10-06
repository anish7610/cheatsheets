# `tzdata` Command Overview

`tzdata` is not a command itself but the package that provides time zone data and tools in Linux. It contains the `timedatectl` command, which is used to query and change system time and settings.

## Common `timedatectl` Options

| Option                  | Description                                   |
|-------------------------|-----------------------------------------------|
| `status`                | Displays current time settings and timezone.  |
| `list-timezones`        | Lists all available timezones.                |
| `set-timezone <zone>`   | Sets the system timezone.                     |
| `set-time <time>`       | Sets the system time.                         |
| `set-local-rtc 0/1`     | Configures RTC (Real-Time Clock) to UTC or local time. |

## Usage Examples

### Display Current Time Settings

```bash
timedatectl status
```

### List All Available Timezones

```bash
timedatectl list-timezones
```

### Set System Timezone to `America/New_York`

```bash
timedatectl set-timezone America/New_York
```

### Set System Time to Specific Value

```bash
timedatectl set-time "2023-10-05 10:00:00"
```

### Configure RTC to Use Local Time

```bash
timedatectl set-local-rtc 1
```

## Cheat Sheet

```plaintext
# Display current time settings
timedatectl status

# List all timezones
timedatectl list-timezones

# Set timezone (replace <zone>)
timedatectl set-timezone <zone>

# Set system time (replace <time>)
timedatectl set-time "<time>"

# Configure RTC to use UTC (0) or local (1)
timedatectl set-local-rtc 0/1
```
