# `hwinfo` Command Overview

`hwinfo` is a command-line tool used to extract detailed information about the hardware configuration of a Linux system. It provides extensive details about the system, including CPUs, memory, disks, USBs, graphics cards, network interfaces, and more.

## Common Options

| Option        | Description                                           |
|---------------|-------------------------------------------------------|
| `--short`     | Provides concise output of the hardware information.  |
| `--cpu`       | Displays information about the CPU.                   |
| `--disk`      | Displays information about disk drives.               |
| `--memory`    | Shows details about system memory.                    |
| `--network`   | Provides information about network interfaces.        |
| `--gfxcard`   | Shows details about the graphics card.                |
| `--usb`       | Displays information about USB devices.               |
| `--help`      | Displays help and usage information.                  |

## Usage Examples

### Get a Concise Summary of the Hardware

```bash
hwinfo --short
```

### Check CPU Details

```bash
hwinfo --cpu
```

### Retrieve Disk Drive Information

```bash
hwinfo --disk
```

### View Network Interface Details

```bash
hwinfo --network
```

### Display Information About USB Devices

```bash
hwinfo --usb
```

## Cheat Sheet

```plaintext
hwinfo --short            # Concise hardware summary
hwinfo --cpu              # CPU information
hwinfo --disk             # Disk drive details
hwinfo --memory           # Memory information
hwinfo --network          # Network interface info
hwinfo --gfxcard          # Graphics card details
hwinfo --usb              # USB device info
```
