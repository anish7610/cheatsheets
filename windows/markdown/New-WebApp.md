# New-WebApp Command

`New-WebApp` is a Windows PowerShell command used to create a new web application in Internet Information Services (IIS). This command helps in setting up a web application by defining its settings and configuration.

## Common Options

| Option                | Explanation                                                    |
|-----------------------|----------------------------------------------------------------|
| `-Name`               | Specifies the name of the new web application.                 |
| `-Site`               | Defines the site under which the web application will be created. |
| `-PhysicalPath`       | Sets the physical path of the web application's root directory. |
| `-ApplicationPool`    | Assigns an application pool for isolation and management.     |

## Usage Examples

### Example 1: Basic Web Application Creation

```shell
New-WebApp -Name "MyApp" -Site "Default Web Site" -PhysicalPath "C:\inetpub\wwwroot\MyApp"
```

### Example 2: Web Application with Custom Application Pool

```shell
New-WebApp -Name "MyApp" -Site "Default Web Site" -PhysicalPath "C:\inetpub\wwwroot\MyApp" -ApplicationPool "MyAppPool"
```

## Cheat Sheet

```plaintext
New-WebApp -Name <AppName> -Site <SiteName> -PhysicalPath <Path> [-ApplicationPool <PoolName>]
```
