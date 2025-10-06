# Get-VM Command Overview

The `Get-VM` command in Windows PowerShell is used to obtain information about virtual machines on a Hyper-V host. It displays details such as VM name, state, and additional configuration settings.

## Common Options

| Option                   | Explanation                                                                   |
|--------------------------|-------------------------------------------------------------------------------|
| `-Name`                  | Specifies the name of the virtual machine to retrieve.                        |
| `-ComputerName`          | Retrieves the VMs from a specified Hyper-V host.                              |
| `-State`                 | Filters VMs by their current state (Running, Stopped, etc.).                  |
| `-Id`                    | Uses the unique identifier to select a VM.                                    |
| `-SwitchName`            | Retrieves VMs connected to a specific virtual switch.                         |
| `-IncludeManagementOS`   | Includes the management operating system in the output.                       |

## Usage Examples

### List all VMs on the local host
```powershell
Get-VM
```

### Find a specific VM by name
```powershell
Get-VM -Name "MyVirtualMachine"
```

### List all VMs on a remote host
```powershell
Get-VM -ComputerName "RemoteHostName"
```

### Show VMs that are currently running
```powershell
Get-VM | Where-Object {$_.State -eq 'Running'}
```

### Retrieve VM information using the VM's ID
```powershell
Get-VM -Id "12345678-1234-1234-1234-123456789abc"
```

### List VMs connected to a specific virtual switch
```powershell
Get-VM -SwitchName "MyVirtualSwitch"
```

## Cheat Sheet

```plaintext
Get-VM                     # List all VMs
Get-VM -Name "VMName"      # Find VM by name
Get-VM -ComputerName "Host"  # VMs on remote host
Get-VM | Where-Object {$_.State -eq 'Running'}  # Running VMs
```
