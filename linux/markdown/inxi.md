# `inxi` Command Overview

`inxi` is a versatile command-line tool for gathering comprehensive system information. It provides a detailed overview of hardware and software configurations, making it useful for diagnostics and reporting.

## Common Options

| Option | Description                                     |
|--------|-------------------------------------------------|
| `-F`   | Full system information                         |
| `-S`   | Basic system information                         |
| `-C`   | CPU details                                     |
| `-m`   | Memory details                                  |
| `-G`   | Graphics information                             |
| `-A`   | Audio/sound information                         |
| `-d`   | Disk information                                |
| `-n`   | Network information                             |
| `-N`   | Advanced network information                    |
| `-r`   | Repositories                                    |
| `-xxx` | Maximum verbosity for detailed outputs          |

## Usage Examples

### Full System Information
```bash
inxi -F
```

### Show CPU Details
```bash
inxi -C
```

### Show Memory Details
```bash
inxi -m
```

### Display Graphics Information
```bash
inxi -G
```

### Network Information
```bash
inxi -n
```

### Detailed Output for Diagnostics
```bash
inxi -Fxxx
```

## Cheat Sheet

```bash
inxi -F    # Full system
inxi -C    # CPU
inxi -m    # Memory
inxi -G    # Graphics
inxi -n    # Network
inxi -Fxxx # Detailed
```
