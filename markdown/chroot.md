# `chroot` Command in Linux

## Description

`chroot` changes the root directory for a process and its children to a specified directory. It creates a confined space, effectively isolating processes from other parts of the filesystem. This is especially useful for building, testing, or repairing systems.

## Common Options

| Option | Description                              |
|--------|------------------------------------------|
| `--userspec=USER:GROUP` | Set the user and group for the command. |
| `--groups=G_LIST`       | Specify supplementary groups.          |
| `--help`                | Display help information.              |
| `--version`             | Output version information.            |

## Usage Examples

### Basic Example

```bash
sudo chroot /mnt/my-chroot
```
Changes the root directory to `/mnt/my-chroot`. Useful for system repairs in a mounted environment.

### With User Specification

```bash
sudo chroot --userspec=1000:1000 /mnt/my-chroot /bin/bash
```
Runs `/bin/bash` in the new root directory with a specific user ID and group ID.

### Running a Command

```bash
sudo chroot /mnt/my-chroot ls /home
```
Lists the contents of `/home` in the new root directory.

## Cheat Sheet

```bash
# Basic Chroot
sudo chroot /new/root

# Chroot with User and Group
sudo chroot --userspec=USER:GROUP /new/root /bin/bash

# Run Command in Chroot
sudo chroot /new/root command

# Help and Version
chroot --help
chroot --version
```
