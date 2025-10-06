# `umount` Command in Linux

The `umount` command is used to unmount filesystems in Linux. It detaches the specified file system from the file hierarchy.

## Common Options

| Option         | Explanation                                   |
|----------------|-----------------------------------------------|
| `-a`           | Unmount all filesystems mentioned in `/etc/mtab`. |
| `-f`           | Force unmount (useful with unreachable NFS systems). |
| `-l`           | Lazy unmount. Detaches the filesystem immediately but cleans when it's no longer busy. |
| `-r`           | Remount as read-only if unmounting fails.     |
| `--help`       | Display a help message with options.          |

## Usage Examples

### Unmount a Single Filesystem
Unmount a specific filesystem by providing the directory where it's mounted:
```bash
umount /mnt/my_drive
```

### Force Unmount
Forcefully unmount a filesystem, useful when the resource is unreachable:
```bash
umount -f /mnt/nfs_share
```

### Lazy Unmount
Detach a busy filesystem now and clean it up after the process terminates:
```bash
umount -l /mnt/usb
```

### Unmount All Filesystems
Unmount all filesystems listed in `/etc/mtab`:
```bash
umount -a
```

## Cheat Sheet

```plaintext
umount [options] <target>
Options:
  -a      Unmount all
  -f      Force unmount
  -l      Lazy unmount
  -r      Remount as read-only if unmount fails
```
