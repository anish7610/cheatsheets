# Get-Disk Command

The `Get-Disk` command in Windows is used to retrieve information about physical disks, including operational status and health.

## Common Options

| Option            | Explanation                                                |
|-------------------|------------------------------------------------------------|
| `-Number <UInt32>`| Specifies a particular disk by its number.                 |
| `-BusType <String>`| Filters the disks by bus type (e.g., USB, SATA).          |
| `-PartitionStyle <String>`| Filters disks by partition style (MBR, GPT).       |
| `-CimSession`     | Runs the command on a remote computer.                     |

## Usage Examples

### List All Disks
```powershell
Get-Disk
```

### Get Information About a Specific Disk
```powershell
Get-Disk -Number 1
```

### List USB Drives Only
```powershell
Get-Disk | Where-Object BusType -eq 'USB'
```

### Display Disks with GPT Partition Style
```powershell
Get-Disk | Where-Object PartitionStyle -eq 'GPT'
```

## Cheat Sheet

- **List all disks:** `Get-Disk`
- **Specific disk:** `Get-Disk -Number <number>`
- **USB disks:** `Get-Disk | Where BusType -eq 'USB'`
- **GPT disks:** `Get-Disk | Where PartitionStyle -eq 'GPT'`
