# Get-PerformanceCounter Command

`Get-PerformanceCounter` is a PowerShell command used in Windows to retrieve performance counter data. Performance counters are a way to monitor various system metrics and performance statistics.

## Common Options

| Option                | Explanation                                                      |
|-----------------------|------------------------------------------------------------------|
| `-Counter`            | Specifies the performance counter to retrieve data from.        |
| `-ListSet`            | Displays available counter sets without retrieving actual data. |
| `-ComputerName`       | Retrieves counter data from a remote computer.                  |
| `-SampleInterval`     | Sets the interval in seconds between samples.                   |
| `-MaxSamples`         | Specifies the number of samples to collect.                     |

## Usage Examples

### Display Available Counter Sets

```powershell
Get-PerformanceCounter -ListSet *
```

### Retrieve Specific Performance Counter Data

```powershell
Get-PerformanceCounter -Counter "\Processor(_Total)\% Processor Time"
```

### Get Performance Data from a Remote Computer

```powershell
Get-PerformanceCounter -Counter "\Memory\Available MBytes" -ComputerName "RemotePC"
```

### Continuous Monitoring with Specific Interval and Sample Count

```powershell
Get-PerformanceCounter -Counter "\Network Interface(*)\Bytes Total/sec" -SampleInterval 10 -MaxSamples 5
```

## Cheat Sheet

```plaintext
- List counter sets: Get-PerformanceCounter -ListSet *
- Specific counter: Get-PerformanceCounter -Counter "\Category\Counter"
- Remote counter data: Get-PerformanceCounter -Counter "\Category\Counter" -ComputerName "PC"
- Set interval/samples: Get-PerformanceCounter -Counter "..." -SampleInterval N -MaxSamples M
```
