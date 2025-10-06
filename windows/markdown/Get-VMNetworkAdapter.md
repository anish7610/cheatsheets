# Get-VMNetworkAdapter Command

`Get-VMNetworkAdapter` is a Windows PowerShell command used to retrieve network adapter configurations for virtual machines on Hyper-V. It provides details such as the adapter's name, IP addresses, VLAN configurations, and more.

## Common Options

| Option                  | Explanation                                               |
|-------------------------|-----------------------------------------------------------|
| `-VMName`               | Specifies the name of the virtual machine to query.       |
| `-VMId`                 | Specifies the unique identifier of the virtual machine.    |
| `-ManagementOS`         | Retrieves network adapters associated with the management OS. |
| `-CimSession`           | Runs the cmdlet on a remote session.                      |
| `-Name`                 | Filters the result based on the network adapter's name.   |

## Usage Examples

### Retrieve All Network Adapters for a VM

```powershell
Get-VMNetworkAdapter -VMName "MyVirtualMachine"
```

### Get Network Adapter for a VM Using VM ID

```powershell
Get-VMNetworkAdapter -VMId "12345-abcde-67890-fghij"
```

### Retrieve Network Adapters for the Management OS

```powershell
Get-VMNetworkAdapter -ManagementOS
```

### Retrieve Specific Network Adapter by Name

```powershell
Get-VMNetworkAdapter -VMName "MyVirtualMachine" -Name "NetworkAdapter1"
```

## Cheat Sheet

```plaintext
Get All Adapters: Get-VMNetworkAdapter -VMName "VMName"
Get By ID:        Get-VMNetworkAdapter -VMId "VMId"
Management OS:    Get-VMNetworkAdapter -ManagementOS
Filter by Name:   Get-VMNetworkAdapter -VMName "VMName" -Name "AdapterName"
```

This quick reference focuses on invoking `Get-VMNetworkAdapter` with different options to suit various common administrative tasks involving VM network configuration in a Hyper-V environment.
