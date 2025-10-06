# `virt-manager` Command Overview

`virt-manager` (Virtual Machine Manager) is a graphical tool for creating and managing virtual machines via `libvirt`. It provides a simplified interface to configure VMs, which can run on local or remote hosts.

## Common Options

| Option                  | Description                                          |
|-------------------------|------------------------------------------------------|
| `-c` `URI`              | Connect to the specified hypervisor at `URI`.        |
| `--no-fork`             | Run in the foreground (don't fork).                  |
| `--debug`               | Enable debug output for troubleshooting.             |
| `-h`, `--help`          | Display help information.                            |

## Usage Examples

### Create a New Virtual Machine
```bash
virt-manager
```
This command opens the Virtual Machine Manager GUI to create and manage virtual machines.

### Connect to a Remote Hypervisor
```bash
virt-manager -c qemu+ssh://remote-server/system
```
Connect to a remote hypervisor using SSH.

### Enable Debug Mode
```bash
virt-manager --debug
```
Start `virt-manager` with debug logging to troubleshoot issues.

## Cheat Sheet

```plaintext
# Start virt-manager
virt-manager

# Connect to a remote VM host
virt-manager -c qemu+ssh://host/system

# Debug mode for issues
virt-manager --debug
```
