# Stop-Job Command in Windows

The `Stop-Job` command is used in Windows PowerShell to stop a running background job. This command is helpful when you need to halt processes that were started asynchronously and are no longer required.

## Common Options

| Option          | Description                                           |
|-----------------|-------------------------------------------------------|
| `-Id`           | Stops the job with the specified ID.                  |
| `-Name`         | Stops the job with the specified name.                |
| `-InstanceId`   | Stops the job with a specific instance ID.            |
| `-Force`        | Forces the job to stop, without confirmation prompts. |

## Usage Examples

### Stop a Job by ID
To stop a job with a specific ID:

```powershell
Stop-Job -Id 3
```

### Stop a Job by Name
To stop a job with a specific name:

```powershell
Stop-Job -Name "DataProcessingJob"
```

### Force Stop a Job
To forcefully stop a job without confirmation:

```powershell
Stop-Job -Id 2 -Force
```

## Cheat Sheet

```plaintext
Stop-Job -Id <JobID>
Stop-Job -Name <JobName>
Stop-Job -InstanceId <InstanceID>
Stop-Job -Id <JobID> -Force
```
