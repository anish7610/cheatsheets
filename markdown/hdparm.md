# `hdparm` Command Overview

`hdparm` is a command-line utility for configuring and displaying information about SATA and IDE devices. It's commonly used for performance tuning and disk parameter querying.

## Common Options

| Option      | Description                                                   |
|-------------|---------------------------------------------------------------|
| `-t`        | Perform a read speed test on the device.                      |
| `-T`        | Perform a cached read speed test.                             |
| `-I`        | Display detailed device information and capabilities.         |
| `-i`        | Show a brief summary of device information.                   |
| `-g`        | Display the geometry (cylinders, heads, sectors) of the disk. |
| `--security-help` | Show security management options.                           |
| `-S`        | Set the standby timeout for the drive (spindown).             |
| `-B`        | Set the Advanced Power Management (APM) level.                |

## Usage Examples

### Check Read Speed
```bash
sudo hdparm -t /dev/sda
```

### Check Cached Read Speed
```bash
sudo hdparm -T /dev/sda
```

### Display Detailed Device Information
```bash
sudo hdparm -I /dev/sda
```

### Display Brief Device Information
```bash
sudo hdparm -i /dev/sda
```

### Set Disk to Spin Down After 5 Minutes of Inactivity
```bash
sudo hdparm -S 60 /dev/sda
```

### Set APM Level to 127
```bash
sudo hdparm -B 127 /dev/sda
```

## Cheat Sheet

```plaintext
# Speed Tests
sudo hdparm -t /dev/sdX      # Measure read speed
sudo hdparm -T /dev/sdX      # Measure cached read speed

# Device Information
sudo hdparm -I /dev/sdX      # Detailed info
sudo hdparm -i /dev/sdX      # Brief info

# Power Management
sudo hdparm -S <val> /dev/sdX # Set standby timeout
sudo hdparm -B <val> /dev/sdX # Set APM level
```

Replace `/dev/sdX` with your specific device identifier.
