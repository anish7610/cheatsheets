# `fstab` Command in Linux

The `/etc/fstab` file is a system configuration file used to define how disk partitions, other block devices, or remote filesystems should be mounted and integrated into the filesystem. It's read by the system at boot time to set up mounts automatically.

## Common Fields in `fstab`

| Field            | Description                                                             |
|------------------|-------------------------------------------------------------------------|
| **Device**       | The UUID or path to the block device.                                   |
| **Mount Point**  | Directory where the device will be mounted.                             |
| **Filesystem**   | Type of filesystem (e.g., ext4, nfs, vfat).                             |
| **Options**      | Mount options (e.g., defaults, noatime, ro).                            |
| **Dump**         | Backup utility indicator (0 to disable).                                |
| **Pass**         | Filesystem check order at boot (0 to disable, 1 for root, 2 for others).|

## Realistic Usage Examples

1. **Mounting an ext4 Partition:**
   ```plaintext
   UUID=123e4567-e89b-12d3-a456-426614174000 /mnt/storage ext4 defaults 0 2
   ```

2. **Mounting a USB Drive with Noatime Option (to improve performance):**
   ```plaintext
   /dev/sdb1 /media/usb vfat noatime,defaults 0 0
   ```

3. **Mounting a Network File System:**
   ```plaintext
   server:/export /mnt/nfs nfs defaults 0 0
   ```

4. **Mounting a Swap Partition:**
   ```plaintext
   /dev/sda2 none swap sw 0 0
   ```

## Cheat Sheet

```plaintext
# fstab Fields
Device          Mount_Point  Filesystem  Options         Dump  Pass
UUID=device_ID  /mount/dir   fs_type     option_list     0     2

# Examples
# Mount ext4
UUID=<uuid>     /mnt/storage ext4        defaults        0     2

# Mount vfat with noatime
/dev/sdb1       /media/usb   vfat        noatime,defaults 0    0

# Mount NFS
server:/export  /mnt/nfs     nfs         defaults        0     0

# Mount swap
/dev/sda2       none         swap        sw              0     0
```
