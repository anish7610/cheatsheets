# Clonezilla Command Overview

## Description

`Clonezilla` is a command-line tool used for disk imaging and cloning. It allows you to perform backup, recovery, and deployment tasks efficiently. Clonezilla supports a variety of file systems and can clone both single machines and larger networks.

## Common Options

| Option         | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `-i`           | Interactive mode.                                                           |
| `-r`           | Restore an image to disk or partition.                                      |
| `-b`           | Run in batch mode for scripted operations.                                  |
| `-q`           | Quiet mode, suppresses routine messages.                                    |
| `-d`           | Clone an entire disk.                                                       |
| `-p[auto|ask]` | Partition options: auto (automatically choose) or ask (prompt for input).   |
| `-j2`          | Save disk image as a zip archive.                                           |
| `-sftparg`     | Use custom SSH options for SFTP transfers.                                  |
| `--ocs-onthefly`| Perform cloning without saving an intermediate image file.                 |
| `--rescue`     | Rescue or recover a broken partition image.                                 |

## Usage Examples

### Clone a Disk to an Image

Clone an entire disk `/dev/sda` to an image stored in `/backup/images`:

```bash
sudo clonezilla -d -i -q /dev/sda /backup/images/image.sda
```

### Restore from an Image

Restore a partition from an image to `/dev/sda1`:

```bash
sudo clonezilla -r -q /backup/images/image.sda1 /dev/sda1
```

### Batch Mode for Automation

Automate disk cloning using batch mode:

```bash
sudo clonezilla -b -d /dev/sda /backup/images/image.sda
```

### Perform On-the-Fly Cloning

Clone a disk directly to another disk:

```bash
sudo clonezilla --ocs-onthefly /dev/sda /dev/sdb
```

## Cheat Sheet

```markdown
# Clone a disk to an image
sudo clonezilla -d -i -q [source] [destination]

# Restore from an image
sudo clonezilla -r -q [image] [destination]

# Batch clone
sudo clonezilla -b -d [source] [destination]

# On-the-Fly cloning
sudo clonezilla --ocs-onthefly [source] [target]
```
