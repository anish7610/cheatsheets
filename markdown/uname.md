## `uname` Command Overview

The `uname` command in Linux is used to print system information. It can display details such as the kernel name, version, hardware architecture, and more.

## Common Options

| Option | Description                           |
|--------|---------------------------------------|
| `-s`   | Prints the kernel name.               |
| `-n`   | Displays the network hostname.        |
| `-r`   | Shows the kernel release.             |
| `-v`   | Outputs the kernel version.           |
| `-m`   | Displays the machine hardware name.   |
| `-p`   | Prints the processor type (if known). |
| `-i`   | Shows the hardware platform (if known).|
| `-o`   | Outputs the operating system name.    |
| `-a`   | Prints all system information.        |

## Usage Examples

- **Print all system information:**
  ```bash
  uname -a
  ```

- **Show the kernel name:**
  ```bash
  uname -s
  ```

- **Display the kernel version:**
  ```bash
  uname -v
  ```

- **Check the machine hardware name:**
  ```bash
  uname -m
  ```

## Cheat Sheet

```bash
uname -a   # All system info
uname -s   # Kernel name
uname -n   # Network hostname
uname -r   # Kernel release
uname -v   # Kernel version
uname -m   # Machine hardware name
uname -p   # Processor type
uname -i   # Hardware platform
uname -o   # Operating system
```
