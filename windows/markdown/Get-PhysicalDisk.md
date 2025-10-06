# Get-PhysicalDisk Command

`Get-PhysicalDisk` is a PowerShell command used to retrieve information about physical disk drives on a Windows system. It provides details such as status, health, and operational characteristics of each physical disk.

## Common Options

| Option | Description |
|--------|-------------|
| `-FriendlyName` | Displays only disks with a specific friendly name. |
| `-CanPool` | Filters the output to show disks that can be added to a storage pool. |
| `-SerialNumber` | Finds a disk using the serial number. |

## Usage Examples

### List All Physical Disks

```powershell
Get-PhysicalDisk
```

### Filter Disks by Friendly Name

```powershell
Get-PhysicalDisk -FriendlyName "Disk 1"
```

### Show Disks That Can Be Pooled

```powershell
Get-PhysicalDisk | Where-Object CanPool -eq $true
```

### Find Disk by Serial Number

```powershell
Get-PhysicalDisk | Where-Object SerialNumber -eq "12345XYZ"
```

## Cheat Sheet

```plaintext
List Disks: Get-PhysicalDisk
Filter by Name: Get-PhysicalDisk -FriendlyName "<name>"
Poolable Disks: Get-PhysicalDisk | Where-Object CanPool -eq $true
Find by Serial: Get-PhysicalDisk | Where-Object SerialNumber -eq "<serial>"
```
