# `vboxmanage` Command

`vboxmanage` is a command-line utility for managing VirtualBox virtual machines. It enables users to create, configure, and control VMs without using the graphical interface.

## Common Options

| Option            | Explanation                                                             |
|-------------------|-------------------------------------------------------------------------|
| `createvm`        | Create a new virtual machine.                                           |
| `startvm`         | Start a virtual machine.                                                |
| `controlvm`       | Control the execution of a running virtual machine (pause, reset, etc.).|
| `list`            | List various aspects, such as running VMs, host information, etc.       |
| `modifyvm`        | Modify settings of an existing virtual machine.                         |
| `showvminfo`      | Display detailed information about a specific virtual machine.          |
| `snapshot`        | Manage VM snapshots (take, restore, delete).                            |

## Usage Examples

### Creating a New VM

```bash
vboxmanage createvm --name "UbuntuVM" --register
```

### Starting a VM

```bash
vboxmanage startvm "UbuntuVM" --type headless
```

### Modifying VM Settings

```bash
vboxmanage modifyvm "UbuntuVM" --memory 2048 --vram 128 --cpus 2
```

### Taking a Snapshot

```bash
vboxmanage snapshot "UbuntuVM" take "InitialSetup"
```

### Listing All VMs

```bash
vboxmanage list vms
```

### Showing VM Information

```bash
vboxmanage showvminfo "UbuntuVM"
```

## Cheat Sheet

```plaintext
# Create a VM
vboxmanage createvm --name "VMName" --register

# Start VM (headless)
vboxmanage startvm "VMName" --type headless

# Modify VM
vboxmanage modifyvm "VMName" --memory 2048 --vram 128 --cpus 2

# Take Snapshot
vboxmanage snapshot "VMName" take "SnapshotName"

# List all VMs
vboxmanage list vms

# Show VM Info
vboxmanage showvminfo "VMName"
```
