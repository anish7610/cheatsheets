# Get-WBJob Command

`Get-WBJob` is a PowerShell command used to retrieve information about backup operations performed on a Windows system. It displays the status and details of backup jobs, including whether they succeeded, failed, or are in progress.

## Common Options

| Option         | Description                                         |
|----------------|-----------------------------------------------------|
| `-Previous`    | Retrieves the backup job that ran prior to the current one. |
| `-All`         | Retrieves all backup jobs available on the system.   |

## Usage Examples

### Example 1: Retrieve the Current Backup Job

```powershell
Get-WBJob
```
*Displays details of the most recent backup job.*

### Example 2: Retrieve the Previous Backup Job

```powershell
Get-WBJob -Previous
```
*Fetches details about the backup job that ran before the current one.*

### Example 3: Retrieve All Backup Jobs

```powershell
Get-WBJob -All
```
*Displays information about all backup jobs on the system.*

## Cheat Sheet

```plaintext
Get-WBJob          # Get current backup job details
Get-WBJob -Previous # Get previous backup job
Get-WBJob -All      # Get all backup jobs
```
