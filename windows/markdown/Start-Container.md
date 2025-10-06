# Start-Container Command

`Start-Container` is a Windows PowerShell command used to start an existing container.

## Common Options

| Option                | Description                                        |
|-----------------------|----------------------------------------------------|
| `-Name`               | Specifies the name of the container to start.      |
| `-Id`                 | Specifies the ID of the container to start.        |
| `-Credential`         | Specifies the user credentials for the container.  |
| `-AsJob`              | Runs the command as a background job.              |

## Usage Examples

### Starting a Container by Name
```powershell
Start-Container -Name "myContainer"
```

### Starting a Container by ID
```powershell
Start-Container -Id "123456789"
```

### Starting a Container as a Background Job
```powershell
Start-Container -Name "myContainer" -AsJob
```

### Starting a Container with Specific Credentials
```powershell
$credential = Get-Credential
Start-Container -Name "myContainer" -Credential $credential
```

## Cheat Sheet

```markdown
Start-Container -Name <container-name>
Start-Container -Id <container-id>
Start-Container -Name <container-name> -AsJob
Start-Container -Name <container-name> -Credential <credential-object>
```
