# PowerShell (for Hyper-V)

PowerShell for Hyper-V allows you to manage Hyper-V virtual machines and their settings through a command-line interface, providing powerful automation and scripting capabilities.

## Common Options

| Option                       | Explanation                                               |
|------------------------------|-----------------------------------------------------------|
| `Get-VM`                     | Retrieves information about virtual machines.             |
| `Start-VM <VMName>`          | Starts a specified virtual machine.                       |
| `Stop-VM <VMName>`           | Stops a specified virtual machine.                        |
| `New-VM -Name <VMName>`      | Creates a new virtual machine with the specified name.    |
| `Remove-VM <VMName>`         | Deletes a specified virtual machine.                      |
| `Set-VM -Name <VMName>`      | Configures settings for an existing virtual machine.      |
| `Checkpoint-VM <VMName>`     | Creates a checkpoint of a specified virtual machine.      |
| `Restore-VMSnapshot <Name>`  | Restores a virtual machine to a specified checkpoint.     |
| `Export-VM <VMName>`         | Exports a virtual machine to a specified location.        |
| `Import-VM`                  | Imports a virtual machine from a specified location.      |

## Usage Examples

### Retrieve a List of Virtual Machines
```powershell
Get-VM
```

### Start a Virtual Machine
```powershell
Start-VM -Name "UbuntuServer"
```

### Stop a Virtual Machine
```powershell
Stop-VM -Name "UbuntuServer" -Force
```

### Create a New Virtual Machine
```powershell
New-VM -Name "TestVM" -MemoryStartupBytes 1GB -BootDevice VHD
```

### Remove a Virtual Machine
```powershell
Remove-VM -Name "OldVM" -Force
```

### Create a Checkpoint
```powershell
Checkpoint-VM -Name "UbuntuServer" -SnapshotName "PreUpdate"
```

### Restore a Checkpoint
```powershell
Restore-VMSnapshot -Name "PreUpdate" -VMName "UbuntuServer"
```

## Cheat Sheet

```plaintext
Get-VM                             # List VMs
Start-VM <VMName>                  # Start a VM
Stop-VM <VMName> -Force            # Stop a VM
New-VM -Name <VMName>              # New VM
Remove-VM <VMName> -Force          # Delete VM
Checkpoint-VM <VMName>             # Create checkpoint
Restore-VMSnapshot -Name <Name>    # Restore checkpoint
```
