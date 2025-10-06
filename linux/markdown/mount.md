# `mount` Command in Linux

The `mount` command in Linux is used to attach different filesystems to a specified directory, making them accessible in the file system hierarchy.

## Common Options

| Option      | Description                                                                          |
|-------------|--------------------------------------------------------------------------------------|
| `-t`        | Specifies the filesystem type (e.g., ext4, ntfs).                                    |
| `-o`        | Provides specific options to be used while mounting (e.g., ro, rw, noexec).          |
| `-a`        | Mounts all filesystems mentioned in `/etc/fstab`.                                    |
| `-r`        | Mounts the filesystem as read-only.                                                  |
| `-U`        | Mounts a filesystem by its UUID.                                                     |
| `-L`        | Mounts a filesystem by its label.                                                    |

## Usage Examples

### Mount a USB Drive
Mount a USB drive located at `/dev/sdb1` to `/mnt/usb`:
```bash
sudo mount /dev/sdb1 /mnt/usb
```

### Mount with Specific Filesystem
Mount an NTFS partition:
```bash
sudo mount -t ntfs /dev/sda3 /mnt/windows
```

### Mount as Read-only
Mount a CD-ROM as read-only:
```bash
sudo mount -t iso9660 -r /dev/cdrom /mnt/cdrom
```

### Use Options to Customize
Mount with specific options such as read-write and noexec:
```bash
sudo mount -o rw,noexec /dev/sdb1 /mnt/usb
```

### Mount All Filesystems in `/etc/fstab`
```bash
sudo mount -a
```

## Cheat Sheet

```plaintext
# Basic mount
sudo mount <source> <directory>

# With filesystem type
sudo mount -t <fstype> <source> <directory>

# Read-only
sudo mount -r <source> <directory>

# Mount by UUID
sudo mount -U <UUID> <directory>

# Mount using options
sudo mount -o <options> <source> <directory>
```

Note: Always ensure the mount point directory exists before using the `mount` command.
