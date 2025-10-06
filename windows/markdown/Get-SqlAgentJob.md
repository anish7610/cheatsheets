# Get-SqlAgentJob Command

The `Get-SqlAgentJob` command is part of the SQL Server module in Windows PowerShell. It retrieves the SQL Server Agent jobs from an instance of SQL Server, allowing for easy management and automation of tasks related to SQL Agent jobs.

## Common Options

| Option               | Description                                                   |
|----------------------|---------------------------------------------------------------|
| `-ServerInstance`    | Specifies the SQL Server instance name.                       |
| `-JobName`           | Filters results to the specified job name.                    |
| `-Credential`        | Specifies the user account for SQL instance login.            |
| `-Force`             | Suppresses confirmation messages.                             |

## Usage Examples

### Retrieve All Jobs from a Server

```powershell
Get-SqlAgentJob -ServerInstance "MyServer\SQLInstance"
```

### Retrieve a Specific Job

```powershell
Get-SqlAgentJob -ServerInstance "MyServer\SQLInstance" -JobName "NightlyBackupJob"
```

### Using Credentials

```powershell
$cred = Get-Credential
Get-SqlAgentJob -ServerInstance "MyServer\SQLInstance" -Credential $cred
```

## Cheat Sheet

```plaintext
Get all jobs: Get-SqlAgentJob -ServerInstance "Server\Instance"
Get specific job: Get-SqlAgentJob -ServerInstance "Server\Instance" -JobName "JobName"
Use credentials: Get-SqlAgentJob -ServerInstance "Server\Instance" -Credential (Get-Credential)
```
