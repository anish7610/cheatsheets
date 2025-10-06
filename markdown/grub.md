# GRUB Command Overview

**GRUB** (GRand Unified Bootloader) is a bootloader used to load and manage different operating systems on a computer. It's responsible for booting the Linux kernel and allowing users to select from multiple boot configurations.

## Common Options

| Option                  | Description                                              |
|-------------------------|----------------------------------------------------------|
| `grub-install`          | Installs GRUB to a specified drive or partition.         |
| `grub-mkconfig`         | Generates a new GRUB configuration file.                 |
| `grub-update`           | Updates GRUB configuration; often a wrapper for `grub-mkconfig`. |
| `-o <FILE>`             | Output the generated configuration to the specified file. |

## Usage Examples

### Install GRUB
Install GRUB to the Master Boot Record (MBR) of `/dev/sda`.
```bash
sudo grub-install /dev/sda
```

### Generate a New Configuration
Create a new configuration file, typically used after upgrading the kernel.
```bash
sudo grub-mkconfig -o /boot/grub/grub.cfg
```

### Update GRUB Configuration
Update GRUB to recognize new kernels or changes.
```bash
sudo update-grub
```

## Cheat Sheet

```plaintext
# Install GRUB to a drive
sudo grub-install /dev/sdX

# Generate GRUB configuration
sudo grub-mkconfig -o /boot/grub/grub.cfg

# Update GRUB (Debian-based systems)
sudo update-grub

# Repair GRUB (in rescue mode)
grub> set prefix=(hd0,msdos1)/grub
grub> set root=(hd0,msdos1)
grub> insmod normal
grub> normal
```
