# `fdisk` Command in Linux

## Description

`fdisk` is a command-line utility for managing disk partitions. It allows you to create, delete, modify, and list partitions on a hard drive.

## Common Options

| Option | Description                               |
|--------|-------------------------------------------|
| `-l`   | List partition tables for all devices.    |
| `-s`   | Display the size of a partition.          |
| `-u`   | Display sizes in sectors (default in Linux). |
| `-n`   | Add a new partition.                      |
| `-d`   | Delete a partition.                       |
| `-v`   | Display the version of `fdisk`.           |

## Usage Examples

### List All Partitions
To list all partitions on all available devices:
```bash
sudo fdisk -l
```

### Display Size of a Partition
To display the size of `/dev/sda1`:
```bash
sudo fdisk -s /dev/sda1
```

### Create a New Partition
To create a new partition on `/dev/sda`:
1. Open `fdisk`:
   ```bash
   sudo fdisk /dev/sda
   ```
2. Enter `n` and follow prompts to create a partition.
3. Write changes with `w`.

### Delete a Partition
To delete a partition on `/dev/sda`:
1. Open `fdisk`:
   ```bash
   sudo fdisk /dev/sda
   ```
2. Enter `d` and select the partition to delete.
3. Write changes with `w`.

## Cheat Sheet

```markdown
# List all partitions
sudo fdisk -l

# Display partition size
sudo fdisk -s /dev/sdXn

# Open fdisk to create/delete partitions
sudo fdisk /dev/sdX

# General Workflow in fdisk
# 1. Create partition: n
# 2. Delete partition: d
# 3. Write changes: w
```

Replace `/dev/sdX` and `/dev/sdXn` with appropriate disk identifiers. Always backup data and ensure accuracy before modifying partitions.
