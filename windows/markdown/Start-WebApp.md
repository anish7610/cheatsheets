# `Start-WebApp` Command

The `Start-WebApp` command is used in the Windows PowerShell environment to start a web application in Internet Information Services (IIS).

## Common Options

| Option              | Explanation                                            |
|---------------------|--------------------------------------------------------|
| `-Name`             | Specifies the name of the web application to start.    |
| `-Site`             | Specifies the site that hosts the web application.     |
| `-Confirm`          | Prompts for confirmation before executing the command. |
| `-WhatIf`           | Shows what would happen if the command runs.           |

## Usage Examples

### Start a Web Application

```powershell
Start-WebApp -Name "MyWebApp" -Site "Default Web Site"
```

### Use `-WhatIf` to Simulate Command Execution

```powershell
Start-WebApp -Name "MyWebApp" -Site "Default Web Site" -WhatIf
```

### Use with Confirmation

```powershell
Start-WebApp -Name "MyWebApp" -Site "Default Web Site" -Confirm
```

## Cheat Sheet

```plaintext
Start-WebApp -Name <AppName> -Site <SiteName> [-Confirm] [-WhatIf]
```

- **Start an app:** `Start-WebApp -Name "MyApp" -Site "MySite"`
- **Simulate:** Add `-WhatIf`
- **Confirm:** Add `-Confirm`
