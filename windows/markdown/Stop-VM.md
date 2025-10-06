# Stop-VM Command

The `Stop-VM` command in Windows PowerShell is used to stop a virtual machine (VM) in Hyper-V. It's equivalent to pulling the power cord, stopping the VM immediately.

## Common Options

| Option           | Description                                        |
|------------------|----------------------------------------------------|
| `-Name`          | Specifies the name of the VM to stop.              |
| `-Force`         | Forcefully stops the VM without confirmation.      |
| `-Passthru`      | Returns the VM object after the operation.         |
| `-WhatIf`        | Shows what would happen if the command is run.     |
| `-Confirm`       | Prompts for confirmation before stopping the VM.   |

## Usage Examples

### Stop a VM by Name

```powershell
Stop-VM -Name "UbuntuVM"
```

### Forcefully Stop a VM

```powershell
Stop-VM -Name "UbuntuVM" -Force
```

### Stop a VM and Return the VM Object

```powershell
Stop-VM -Name "UbuntuVM" -Passthru
```

### Check What Would Happen

```powershell
Stop-VM -Name "UbuntuVM" -WhatIf
```

## Cheat Sheet

```plaintext
Stop-VM -Name "VMName"           # Stop a VM by name
Stop-VM -Name "VMName" -Force    # Forcefully stop a VM
Stop-VM -Name "VMName" -Passthru # Get VM object after stopping
Stop-VM -Name "VMName" -WhatIf   # Display action without executing
```
