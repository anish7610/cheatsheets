# Get-WBPolicy Command

`Get-WBPolicy` is a PowerShell cmdlet used to retrieve the current backup policy on a Windows system. It is part of the Windows Server Backup feature and helps manage backup settings.

## Common Options

| Option | Description                                   |
|--------|-----------------------------------------------|
| N/A    | No specific options; retrieves the backup policy. |

## Usage Examples

### Retrieve Current Backup Policy

```powershell
Get-WBPolicy
```

Displays the current backup policy settings, including what items are being backed up and the schedule.

### Retrieve and Display as List

```powershell
Get-WBPolicy | Format-List
```

Outputs the backup policy details in a list format for better readability.

## Cheat Sheet

- **View Current Backup Policy**:
  ```powershell
  Get-WBPolicy
  ```
- **Format Output as List**:
  ```powershell
  Get-WBPolicy | Format-List
  ```

Make sure the Windows Server Backup feature is installed to use this cmdlet.
