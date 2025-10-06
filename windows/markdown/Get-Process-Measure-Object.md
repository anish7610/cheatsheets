# `Get-Process | Measure-Object`

The command `Get-Process | Measure-Object` in Windows PowerShell retrieves all running processes and uses the `Measure-Object` cmdlet to calculate statistics like count, average, sum, etc., on those processes.

## Common Options

| Option     | Explanation                                           |
|------------|-------------------------------------------------------|
| `-Property`| Specifies the property to measure (e.g., `WorkingSet`)|
| `-Sum`     | Calculates the sum of the values of the specified property |
| `-Average` | Calculates the average of the values of the specified property |
| `-Minimum` | Finds the minimum value of the specified property     |
| `-Maximum` | Finds the maximum value of the specified property     |
| `-Count`   | Counts the number of objects                          |

## Usage Examples

### Count All Running Processes

```powershell
Get-Process | Measure-Object
```

### Sum of Working Set Memory

```powershell
Get-Process | Measure-Object -Property WorkingSet -Sum
```

### Calculate Average and Max CPU Usage

```powershell
Get-Process | Measure-Object -Property CPU -Average -Maximum
```

### Find Minimum and Maximum Handles Used

```powershell
Get-Process | Measure-Object -Property Handles -Minimum -Maximum
```

## Cheat Sheet

```plaintext
# Count processes
Get-Process | Measure-Object

# Sum a property (e.g., memory)
Get-Process | Measure-Object -Property WorkingSet -Sum

# Average and Max CPU usage
Get-Process | Measure-Object -Property CPU -Average -Maximum

# Min and Max Handles
Get-Process | Measure-Object -Property Handles -Minimum -Maximum
```
