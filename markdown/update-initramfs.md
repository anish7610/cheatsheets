## Overview of `update-initramfs`

`update-initramfs` is a Linux command used to create, update, or delete the initial RAM filesystem (`initramfs`) images, which are crucial for booting Debian-based systems.

## Common Options

| Option        | Description                                                                              |
|---------------|------------------------------------------------------------------------------------------|
| `-c`          | Create a new initramfs image. Requires specifying a kernel version with the `-k` option. |
| `-u`          | Update an existing initramfs image. By default, for the running kernel.                   |
| `-d`          | Delete an existing initramfs image.                                                       |
| `-k VERSION`  | Specify the kernel version for which the initramfs image should be created, updated, or deleted. |
| `-b DIR`      | Set an alternate boot directory.                                                          |
| `-v`          | Enable verbose mode for more detailed output.                                             |

## Usage Examples

### Creating a New Initramfs for a Specific Kernel
```bash
sudo update-initramfs -c -k 5.10.0-14-generic
```

### Updating the Initramfs for the Default (Running) Kernel
```bash
sudo update-initramfs -u
```

### Deleting an Initramfs for a Specific Kernel
```bash
sudo update-initramfs -d -k 5.10.0-13-generic
```

### Updating an Initramfs with Verbose Output
```bash
sudo update-initramfs -u -v
```

## Cheat Sheet

```bash
# Create new initramfs
sudo update-initramfs -c -k <version>

# Update current initramfs
sudo update-initramfs -u

# Delete specific initramfs
sudo update-initramfs -d -k <version>

# Use verbose mode
sudo update-initramfs -u -v
```
