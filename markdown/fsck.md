# fsck Command in Linux

`fsck` (File System Consistency Check) is a utility used to check and repair file system inconsistencies on Linux disks. It can be run manually or automatically during system boot.

## Common Options

| Option          | Description                                                |
|-----------------|------------------------------------------------------------|
| `-A`            | Check all filesystems in `/etc/fstab`.                     |
| `-C`            | Display progress information.                              |
| `-N`            | Show what would be done, but do not execute actions.       |
| `-R`            | Skip the root filesystem (use with `-A`).                  |
| `-T`            | Do not display the title (header) on start-up.             |
| `-V`            | Verbose mode; shows more detailed output.                  |
| `-y`            | Automatically answer "yes" to prompts for repairs.         |
| `-n`            | Open the filesystem read-only and answer "no" to prompts.  |

## Usage Examples

### Check and Repair a Specific Filesystem
```bash
sudo fsck /dev/sda1
```

### Check All Filesystems Listed in `/etc/fstab`
```bash
sudo fsck -A
```

### Verbose Check of a Filesystem Without Making Changes
```bash
sudo fsck -N -V /dev/sda1
```

### Automatically Repair All Filesystems
```bash
sudo fsck -A -y
```

## Cheat Sheet

```plaintext
fsck /dev/sdXY     - Check and repair a specific filesystem.
fsck -A            - Check all filesystems from fstab.
fsck -A -y         - Auto repair all filesystems.
fsck -N            - Show actions without executing.
fsck -V            - Verbose output.
```

> **Note**: Always unmount the filesystem before running `fsck` or use it in a read-only manner to prevent data corruption.
