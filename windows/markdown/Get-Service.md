# Get-Service Command Overview

`Get-Service` is a PowerShell cmdlet used to retrieve the status of services on a Windows system. It provides details such as service name, display name, and status.

## Common Options

| Option                     | Explanation                                         |
|----------------------------|-----------------------------------------------------|
| `-Name`                    | Specifies the service name. Wildcards accepted.     |
| `-DisplayName`             | Filters services by their display name.             |
| `-Status`                  | Filters services based on their status (Running, Stopped). |
| `-ComputerName`            | Retrieves services from a remote computer.          |
| `-DependentServices`       | Lists services depending on a specific service.     |
| `-RequiredServices`        | Lists services required by a specific service.      |
| `-Exclude`                 | Excludes specific services from the results.        |

## Usage Examples

### List All Services

```shell
Get-Service
```

### Filter Services By Name

```shell
Get-Service -Name 'win*'
```

### Check Status of a Specific Service

```shell
Get-Service -Name 'wuauserv'
```

### List Services That are Running

```shell
Get-Service -Status Running
```

### List Services on a Remote Computer

```shell
Get-Service -ComputerName 'RemotePC'
```

## Quick Reference Cheat Sheet

```markdown
# List All Services
Get-Service

# Filter by Name (supports wildcards)
Get-Service -Name 'win*'

# Check Specific Service
Get-Service -Name 'wuauserv'

# Running Services
Get-Service -Status Running

# Remote Computer Services
Get-Service -ComputerName 'RemotePC'
```
