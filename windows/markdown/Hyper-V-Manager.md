# Hyper-V Manager

## Description

Hyper-V Manager is a Windows tool that provides a graphical interface for managing Hyper-V virtual environments. It allows users to create, configure, and monitor virtual machines (VMs) and other virtual resources.

## Common Options

| Option                  | Explanation                                               |
|-------------------------|-----------------------------------------------------------|
| **Create Virtual Machine** | Wizard to create a new VM.                                |
| **Connect**             | Open a console session with a virtual machine.            |
| **Settings**            | Access and modify configuration settings of a VM.         |
| **Checkpoints**         | Manage snapshots of VM states.                            |
| **Import Virtual Machine** | Import existing VMs from exported files.                   |
| **Virtual Switch Manager** | Configure networking switches for VMs.                    |
| **Hyper-V Settings**    | Adjust general settings for Hyper-V services.             |

## Usage Examples

### Create a New Virtual Machine

1. Open **Hyper-V Manager**.
2. Select **New** > **Virtual Machine** from the Actions pane.
3. Follow the wizard to specify configuration details.

### Connect to a Virtual Machine

- Right-click on the VM name and select **Connect** to open a console session.

### Take a Checkpoint

- Right-click on a running VM and choose **Checkpoint** to save its current state.

### Import a Virtual Machine

1. Select **Import Virtual Machine** from the Actions pane.
2. Follow the wizard to locate and import the VM files.

### Configure a Virtual Switch

1. Click on **Virtual Switch Manager** in the Actions pane.
2. Create a new switch or modify existing ones for VM networking.

## Cheat Sheet

```plaintext
- Create VM: New > Virtual Machine
- Connect to VM: Right-click VM > Connect
- Configure VM: Right-click VM > Settings
- Take Snapshot: Right-click VM > Checkpoint
- Import VM: Actions > Import Virtual Machine
- Network Setup: Actions > Virtual Switch Manager
```
