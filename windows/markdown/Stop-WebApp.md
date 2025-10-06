# Stop-WebApp Command Cheat Sheet

## Description
`Stop-WebApp` is a PowerShell command used to stop a web application in Microsoft IIS (Internet Information Services). It is typically used to halt the deployment of a web application without uninstalling it.

## Common Options

| Option             | Description                                         |
|--------------------|-----------------------------------------------------|
| `-Name <string>`   | Specifies the name of the web application to stop.  |
| `-Passthru`        | Returns an object representing the application.     |
| `-WhatIf`          | Displays what would happen if the command runs.     |
| `-Confirm`         | Prompts for confirmation before stopping the app.   |

## Usage Examples

### Stop a Web Application by Name
```bash
Stop-WebApp -Name "MyWebApp"
```

### Stop with Confirmation
```bash
Stop-WebApp -Name "MyWebApp" -Confirm
```

### Simulate the Stop Command
```bash
Stop-WebApp -Name "MyWebApp" -WhatIf
```

### Stop and Return Object
```bash
Stop-WebApp -Name "MyWebApp" -Passthru
```

## Quick Reference
```plaintext
Stop-WebApp -Name "<AppName>"
Stop-WebApp -Name "<AppName>" -Confirm
Stop-WebApp -Name "<AppName>" -WhatIf
Stop-WebApp -Name "<AppName>" -Passthru
```
