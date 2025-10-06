# Get-Container Command

The `Get-Container` command in Windows PowerShell retrieves information about container instances present on the system. It is part of the container management cmdlets, often used in environments running Windows Containers.

## Common Options

| Option               | Explanation                                            |
|----------------------|--------------------------------------------------------|
| `-Name <String>`     | Filters the containers by the specified name.          |
| `-Id <String>`       | Retrieves containers based on their ID.                |
| `-IncludeStopped`    | Includes containers that are currently stopped.        |
| `-Verbose`           | Provides detailed output information.                  |

## Usage Examples

### List All Containers
```powershell
Get-Container
```

### List a Specific Container by Name
```powershell
Get-Container -Name "myContainer"
```

### Retrieve Container by ID
```powershell
Get-Container -Id "123456789abcdef"
```

### List All Containers Including Stopped Ones
```powershell
Get-Container -IncludeStopped
```

### Detailed Output
```powershell
Get-Container -Verbose
```

## Cheat Sheet

```plaintext
# List all containers
Get-Container

# Filter by name
Get-Container -Name <ContainerName>

# Filter by ID
Get-Container -Id <ContainerID>

# Include stopped containers
Get-Container -IncludeStopped

# Verbose output
Get-Container -Verbose
```
