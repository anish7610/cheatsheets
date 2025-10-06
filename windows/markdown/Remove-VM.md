# Remove-VM Command in Windows

The `Remove-VM` command is used in Windows PowerShell to delete a virtual machine (VM) from a Hyper-V host. This command helps manage and maintain virtual environments by removing unwanted or obsolete VMs.

## Common Options

| Option                 | Explanation                                                        |
|------------------------|--------------------------------------------------------------------|
| `-Name <String>`       | Specifies the name of the VM to remove.                            |
| `-ComputerName <String>` | Specifies the Hyper-V host on which the VM resides.              |
| `-Force`               | Forces the command to execute without prompting for confirmation. |
| `-WhatIf`              | Displays what would happen if the command runs, without executing it. |
| `-Confirm`             | Prompts for confirmation before executing the command.            |

## Usage Examples

### Remove a Specific VM

Remove a VM named "TestVM":

```powershell
Remove-VM -Name "TestVM"
```

### Remove a VM on a Specific Host

Remove a VM named "TestVM" on a Hyper-V host "Host01":

```powershell
Remove-VM -Name "TestVM" -ComputerName "Host01"
```

### Force Removal Without Confirmation

Forcefully remove a VM named "TestVM" without any prompts:

```powershell
Remove-VM -Name "TestVM" -Force
```

### Display Potential Removal Results

Show what would happen if the VM "TestVM" is removed, without actually removing it:

```powershell
Remove-VM -Name "TestVM" -WhatIf
```

## Cheat Sheet

```plaintext
# Basic removal
Remove-VM -Name "<VM_Name>"

# Removal with specified host
Remove-VM -Name "<VM_Name>" -ComputerName "<Host_Name>"

# Force removal
Remove-VM -Name "<VM_Name>" -Force

# Simulate removal
Remove-VM -Name "<VM_Name>" -WhatIf
```

Use this command to efficiently manage VMs on Hyper-V by removing those no longer needed, ensuring a clean and organized virtual environment.
