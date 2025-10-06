# `kvm` Command in Linux

## Description

KVM (Kernel-based Virtual Machine) is a virtualization module in the Linux kernel that allows the kernel to function as a hypervisor. The `kvm` command interfaces with these capabilities to create and manage virtual machines (VMs).

## Common Options

| Option            | Explanation                                         |
|-------------------|-----------------------------------------------------|
| `-m <size>`       | Allocate memory size for the VM (e.g., `-m 1024` for 1GB). |
| `-smp <n>`        | Number of CPU cores allocated to the VM.            |
| `-hda <file>`     | Specify hard disk image file for the VM.            |
| `-cdrom <file>`   | Use a CD-ROM image file to boot the VM.             |
| `-boot <order>`   | Boot the VM in a specified order (e.g., `cd`, `hdd`). |
| `-vnc <display>`  | Enable VNC access to the VM display.                |

## Usage Examples

### Launch a VM with 1GB RAM, 2 CPU cores, and a disk image

```bash
kvm -m 1024 -smp 2 -hda disk.img
```

### Boot a VM from a CD-ROM image

```bash
kvm -cdrom ubuntu.iso -boot d -m 2048
```

### Start a VM with VNC access

```bash
kvm -hda disk.img -m 512 -smp 1 -vnc :1
```

## Cheat Sheet

```plaintext
kvm -m <size> -smp <n> -hda <file>  # Start VM with memory and CPU
kvm -cdrom <file> -boot d           # Boot VM from CD-ROM
kvm -vnc <display>                  # Enable VNC for VM
```
