# mkinitramfs Command

`mkinitramfs` is a utility used to create an initial RAM filesystem (initramfs) for booting a Linux system. It packages essential files and drivers needed during the early boot process, especially when the root filesystem is not directly accessible (e.g., encrypted or located on a network).

## Common Options

| Option         | Description                                                   |
|----------------|---------------------------------------------------------------|
| `-o <file>`    | Specify the output file for the initramfs image.              |
| `-v`           | Enable verbose mode, providing more detailed output.          |
| `-k`           | Keep the temporary directory used during creation.            |
| `-d`           | Dry run; show what would be done without actually doing it.   |
| `-b <dir>`     | Specify an alternate directory for temporary files.           |

## Usage Examples

### Create a Default Initramfs

```bash
sudo mkinitramfs -o /boot/initrd.img-$(uname -r) $(uname -r)
```

### Create Verbose Output of Initramfs

```bash
sudo mkinitramfs -v -o /boot/initrd.img-$(uname -r) $(uname -r)
```

### Specify a Custom Temporary Directory

```bash
sudo mkinitramfs -b /tmp/mytempdir -o /boot/initrd.img-$(uname -r) $(uname -r)
```

### Dry Run to Test Configuration

```bash
sudo mkinitramfs -d -o /boot/initrd.img-$(uname -r) $(uname -r)
```

## Cheat Sheet

```plaintext
Create default initramfs: mkinitramfs -o /boot/initrd.img-$(uname -r) $(uname -r)
Verbose output: mkinitramfs -v -o /boot/initrd.img-$(uname -r) $(uname -r)
Custom temp dir: mkinitramfs -b /custom/dir -o /boot/initrd.img-$(uname -r) $(uname -r)
Dry run: mkinitramfs -d -o /boot/initrd.img-$(uname -r) $(uname -r)
```
