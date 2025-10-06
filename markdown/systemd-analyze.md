# `systemd-analyze` Command Overview

`systemd-analyze` is a command-line utility used to retrieve and display performance statistics about the system's boot process, including startup times and service dependencies.

## Common Options

| Option                   | Description                                                      |
|--------------------------|------------------------------------------------------------------|
| `blame`                  | Shows a list of services ordered by time taken for initialization. |
| `critical-chain`         | Displays the chain of units contributing the most to boot time.  |
| `plot`                   | Generates a graphical representation of the boot process.        |
| `dump`                   | Prints the server's state in a human-readable form.              |
| `time`                   | Provides an overview of the total boot-up time.                  |

## Usage Examples

### Show Services Time Usage
```bash
systemd-analyze blame
```

### Display Critical Chain
```bash
systemd-analyze critical-chain
```

### Generate Boot Process Plot
```bash
systemd-analyze plot > boot.svg
```

### Dump Current Systemd State
```bash
systemd-analyze dump
```

### Get Total Boot Time
```bash
systemd-analyze time
```

## Cheat Sheet

```bash
# View services ordered by startup time
systemd-analyze blame

# Display the critical chain of services affecting boot time
systemd-analyze critical-chain

# Create an SVG plot of the boot process
systemd-analyze plot > boot.svg

# Dump the current state of systemd
systemd-analyze dump

# Check overall system boot-up time
systemd-analyze time
```
