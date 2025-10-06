# GRUB2 Command in Linux

## Description

`grub2` is the default bootloader for most Linux distributions. It allows users to choose which operating system or kernel version to boot.

## Common Options

| Option              | Explanation                                                       |
|---------------------|-------------------------------------------------------------------|
| `grub2-install`     | Installs GRUB2 to a device to enable booting.                     |
| `grub2-mkconfig`    | Generates a new `grub.cfg` configuration file.                    |
| `grub2-editenv`     | Modifies the GRUB environment block.                              |
| `grub2-set-default` | Sets the default boot entry.                                      |
| `grub2-reboot`      | Reboots the system into a specified boot entry just once.         |

## Usage Examples

### Install GRUB2 to a Disk
```bash
sudo grub2-install /dev/sda
```

### Generate a New GRUB Configuration File
```bash
sudo grub2-mkconfig -o /boot/grub2/grub.cfg
```

### Set the Default Boot Entry
```bash
sudo grub2-set-default 1
```

### Reboot into a Specific Boot Entry
```bash
sudo grub2-reboot 2
```

## Cheat Sheet

```plaintext
# Install GRUB2
grub2-install /dev/sdX

# Generate config
grub2-mkconfig -o /boot/grub2/grub.cfg

# Set default
grub2-set-default [entry]

# Temporary reboot to entry
grub2-reboot [entry]
```

Replace `/dev/sdX` and `[entry]` with the appropriate disk and boot entry number.
