# `smartctl` Command

`smartctl` is a command-line utility used to control and monitor storage devices using SMART (Self-Monitoring, Analysis, and Reporting Technology). It's useful for checking the health of hard drives and SSDs.

## Common Options

| Option      | Description                                                        |
|-------------|--------------------------------------------------------------------|
| `-i`        | Displays detailed information about the drive.                     |
| `-a`        | Provides all SMART information, including health, attributes, and errors.|
| `-H`        | Shows the health status of the device.                             |
| `-t short`  | Initiates a short self-test on the device.                         |
| `-t long`   | Initiates a long self-test on the device.                          |
| `-l error`  | Lists the SMART error log.                                         |
| `-l selftest` | Displays the self-test log.                                      |
| `-x`        | Outputs all SMART data, often used for thorough diagnostics.       |

## Usage Examples

### Check Drive Health
```bash
smartctl -H /dev/sda
```

### Display All SMART Information
```bash
smartctl -a /dev/sda
```

### Start a Short Self-Test
```bash
smartctl -t short /dev/sda
```

### View Error Log
```bash
smartctl -l error /dev/sda
```

### Display Self-Test Log
```bash
smartctl -l selftest /dev/sda
```

## Cheat Sheet
```bash
smartctl -H /dev/sdX         # Check health
smartctl -a /dev/sdX         # All SMART info
smartctl -t short /dev/sdX   # Start short test
smartctl -t long /dev/sdX    # Start long test
smartctl -l error /dev/sdX   # Error log
```
Replace `/dev/sdX` with your actual device identifier, such as `/dev/sda`.
