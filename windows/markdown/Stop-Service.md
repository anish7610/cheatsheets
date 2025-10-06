# Stop-Service Command in Windows

The `Stop-Service` command in Windows is used to stop a running service on a local or remote machine. It is commonly used by system administrators to manage services without using the graphical interface.

## Common Options

| Option                  | Explanation                                      |
|-------------------------|--------------------------------------------------|
| `-Name`                 | Specifies the service name to stop.              |
| `-DisplayName`          | Stops services with the specified display name.  |
| `-InputObject`          | Specifies the service object to stop.            |
| `-Force`                | Forces the service to stop.                      |
| `-PassThru`             | Returns an object that represents the service.   |
| `-WhatIf`               | Shows what would happen if the command is run.   |
| `-Confirm`              | Prompts for confirmation before stopping.        |

## Usage Examples

### 1. Stop a Service by Name

```shell
Stop-Service -Name "Spooler"
```

Stops the Printer Spooler service.

### 2. Force Stop a Service

```shell
Stop-Service -Name "W32Time" -Force
```

Forcefully stops the Windows Time service.

### 3. Stop a Service Using Display Name

```shell
Stop-Service -DisplayName "Windows Update"
```

Stops the Windows Update service.

### 4. Stop Multiple Services

```shell
"Spooler", "W32Time" | Stop-Service
```

Stops the Printer Spooler and Windows Time services.

### 5. Simulate the Stop Action

```shell
Stop-Service -Name "Spooler" -WhatIf
```

Displays what would occur if the Spooler service is stopped.

## Cheat Sheet

```plaintext
Stop-Service -Name <ServiceName>                      # Stop service by name
Stop-Service -DisplayName <DisplayName>               # Stop service by display name
Stop-Service -Name <ServiceName> -Force               # Force stop service
Stop-Service -Name <ServiceName> -WhatIf              # Simulate stop action
```
