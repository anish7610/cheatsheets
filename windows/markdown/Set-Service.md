# Set-Service Command

The `Set-Service` command in Windows PowerShell is used to modify the properties of a service on a local or remote computer. It allows you to change the service status, startup type, display name, and other properties.

## Common Options

| Option         | Description                                           |
|----------------|-------------------------------------------------------|
| `-Name`        | Specifies the name of the service.                    |
| `-Status`      | Sets the status of the service (`Running`, `Stopped`).|
| `-StartupType` | Configures the startup type (`Automatic`, `Manual`, `Disabled`).  |
| `-DisplayName` | Sets a user-friendly name for the service.            |
| `-PassThru`    | Returns an object representing the service.           |
| `-ComputerName`| Specifies the remote computer name.                   |

## Usage Examples

### Start a Service

Start the `wuauserv` (Windows Update) service:
```shell
Set-Service -Name "wuauserv" -Status Running
```

### Stop a Service

Stop the `spooler` (Print Spooler) service:
```shell
Set-Service -Name "spooler" -Status Stopped
```

### Change Startup Type

Set the `bits` (Background Intelligent Transfer Service) to start manually:
```shell
Set-Service -Name "bits" -StartupType Manual
```

### Rename Display Name

Change the display name of a service:
```shell
Set-Service -Name "wuauserv" -DisplayName "Windows Update Service"
```

### Remote Computer

Run `Set-Service` on a remote computer named `Server01`:
```shell
Set-Service -Name "spooler" -Status Stopped -ComputerName "Server01"
```

## Cheat Sheet

```shell
Set-Service -Name "<ServiceName>" -Status <Running|Stopped>
Set-Service -Name "<ServiceName>" -StartupType <Automatic|Manual|Disabled>
Set-Service -Name "<ServiceName>" -DisplayName "<NewName>"
Set-Service -Name "<ServiceName>" -Status <Status> -ComputerName "<RemotePC>"
```

Keep this guide handy to efficiently administer services on your Windows machines using PowerShell!
