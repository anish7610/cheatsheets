# Get-PnpDevice Command

`Get-PnpDevice` is a PowerShell cmdlet on Windows used to retrieve information about Plug and Play (PnP) devices on a system. It allows you to query various properties and states of hardware connected to the machine.

## Common Options

| Option                     | Description                                                                 |
|----------------------------|-----------------------------------------------------------------------------|
| `-Class`                   | Filters the devices by class, such as `USB` or `NET`.                       |
| `-FriendlyName`            | Filters devices by a human-readable name.                                   |
| `-InstanceId`              | Specifies the identifier of the device instance to search for.              |
| `-Status`                  | Filters by device status, such as `OK` or `Error`.                          |
| `-PresentOnly`             | Returns only devices that are currently present in the system.              |
| `-Manufacturer`            | Filters devices by manufacturer name.                                       |
| `-EnumeratorName`          | Filters by the name of the enumerator, such as `PCI` or `USB`.              |

## Usage Examples

### List All Devices

```powershell
Get-PnpDevice
```

### List Only USB Devices

```powershell
Get-PnpDevice -Class USB
```

### List Devices with Status Error

```powershell
Get-PnpDevice -Status Error
```

### List Devices with a Specific Friendly Name

```powershell
Get-PnpDevice -FriendlyName 'Intel(R) Wireless Adapter'
```

### List Devices from a Specific Manufacturer

```powershell
Get-PnpDevice -Manufacturer 'NVIDIA'
```

## Cheat Sheet

```plaintext
Get-PnpDevice                 # List all PnP devices
Get-PnpDevice -Class USB      # Filter by class
Get-PnpDevice -Status OK      # Filter by status
Get-PnpDevice -FriendlyName 'Name' # Filter by friendly name
```
