### Get-SqlAgentJobHistory Command Overview

`Get-SqlAgentJobHistory` is a PowerShell cmdlet used to retrieve the history of SQL Server Agent jobs. It provides detailed information about past executions, such as start and end times, outcomes, and job duration.

### Common Options

| Option                  | Explanation                                                  |
|-------------------------|--------------------------------------------------------------|
| `-JobName`              | Specifies the name of the SQL Agent job to retrieve history for. |
| `-SqlInstance`          | Specifies the SQL Server instance to connect to.             |
| `-StartDate`            | Filters the history entries that started on or after this date. |
| `-EndDate`              | Filters the history entries that ended on or before this date. |
| `-OutcomeType`          | Filters entries by job outcome (e.g., Succeeded, Failed).    |
| `-MaxEvents`            | Limits the number of returned history entries.               |

### Usage Examples

#### Example 1: Retrieve History for a Specific Job
```powershell
Get-SqlAgentJobHistory -SqlInstance "ServerName" -JobName "BackupDatabaseJob"
```

#### Example 2: Filter by Date Range
```powershell
Get-SqlAgentJobHistory -SqlInstance "ServerName" -StartDate "2023-01-01" -EndDate "2023-01-31"
```

#### Example 3: Limit Results and Filter by Outcome
```powershell
Get-SqlAgentJobHistory -SqlInstance "ServerName" -JobName "IndexOptimize" -OutcomeType "Succeeded" -MaxEvents 10
```

### Cheat Sheet

```plaintext
# Get history for specific job
Get-SqlAgentJobHistory -SqlInstance "ServerName" -JobName "JobName"

# Filter by start and end dates
Get-SqlAgentJobHistory -SqlInstance "ServerName" -StartDate "YYYY-MM-DD" -EndDate "YYYY-MM-DD"

# Limit events and filter by outcome
Get-SqlAgentJobHistory -SqlInstance "ServerName" -JobName "JobName" -OutcomeType "Outcome" -MaxEvents N
```

Use this command to efficiently manage and monitor SQL Agent job histories in your environment.
