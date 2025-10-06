## Get-Partition Command

`Get-Partition` is a Windows PowerShell cmdlet that retrieves information about the partitions of a disk, including details such as partition size, type, and status.

### Common Options

| Option          | Description                                                                            |
|-----------------|----------------------------------------------------------------------------------------|
| `-DiskNumber`   | Specifies the disk number to get the partitions from.                                   |
| `-PartitionNumber` | Specifies a particular partition number on a disk to retrieve.                    |
| `-CimSession`   | Runs the cmdlet in a session on a remote computer.                                      |
| `-PipelineVariable` | Stores output in a variable for use in subsequent commands in a pipeline.         |

### Usage Examples

#### List All Partitions on Disk 0
```powershell
Get-Partition -DiskNumber 0
```

#### Get Specific Partition Information
```powershell
Get-Partition -DiskNumber 0 -PartitionNumber 1
```

#### Use on a Remote Computer
```powershell
Get-Partition -DiskNumber 0 -CimSession RemotePC
```

### Compact Cheat Sheet

```powershell
# Get all partitions on Disk 0
Get-Partition -DiskNumber 0

# Get details of Partition 1 on Disk 0
Get-Partition -DiskNumber 0 -PartitionNumber 1

# Run on a remote computer
Get-Partition -DiskNumber 0 -CimSession RemotePC
```

Use these commands to efficiently manage and view partition information in your Windows environment.
