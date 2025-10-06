# `free` Command in Linux

The `free` command provides information about the system's memory usage, including total, used, and available memory.

## Common Options

| Option      | Description                                    |
|-------------|------------------------------------------------|
| `-h`        | Display sizes in a human-readable format.      |
| `-m`        | Show memory usage in megabytes.                |
| `-g`        | Show memory usage in gigabytes.                |
| `-s` (sec)  | Continuously display memory usage every `sec` seconds. |
| `-t`        | Display a line showing the total of all columns. |

## Examples

### Display Memory in Human-Readable Format
```bash
free -h
```

### Show Memory in Megabytes
```bash
free -m
```

### Continuously Update Every 5 Seconds
```bash
free -s 5
```

### Display Total Memory Line
```bash
free -t
```

## Cheat Sheet

```bash
free -h      # Human-readable format
free -m      # Display in MB
free -g      # Display in GB
free -s 5    # Update every 5 seconds
free -t      # Show totals
```
