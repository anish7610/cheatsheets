## `Start-VM` Command Overview

The `Start-VM` command is used in Windows PowerShell to start a virtual machine managed by Hyper-V. It's a straightforward command that initiates the operation of specified VMs.

### Common Options

| Option              | Description                                     |
|---------------------|-------------------------------------------------|
| `-Name`             | Specifies the name of the virtual machine to start. |
| `-Id`               | Specifies the GUID of the virtual machine.      |
| `-AsJob`            | Runs the operation as a background job.         |
| `-Passthru`         | Returns an object representing the VM.          |
| `-CimSession`       | Runs the command on a remote session.           |
| `-ComputerName`     | Specifies the Hyper-V host to target.           |

### Examples

#### Starting a VM by Name

```powershell
Start-VM -Name "UbuntuVM"
```

#### Starting a VM by ID

```powershell
Start-VM -Id "f12a8b7d-9f00-48b9-a988-6a557a6b750a"
```

#### Starting a VM on a Remote Host

```powershell
Start-VM -Name "TestVM" -ComputerName "RemoteHVHost"
```

#### Starting a VM as a Background Job

```powershell
Start-VM -Name "LinuxTest" -AsJob
```

### Cheat Sheet

```
Start-VM -Name <VMName>         # Start a VM by its name
Start-VM -Id <VMId>             # Start a VM by its GUID
Start-VM -AsJob                 # Start a VM as a job
Start-VM -ComputerName <Host>   # Start a VM on a remote host
```

This quick guide provides an efficient overview of the `Start-VM` command for managing Hyper-V virtual machines.
