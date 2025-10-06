# Get-WebApplication Command

`Get-WebApplication` is a PowerShell command used to retrieve information about web applications hosted on an IIS (Internet Information Services) server. It provides essential details such as the application’s name, physical path, and associated application pool.

## Common Options

| Option            | Description                                              |
|-------------------|----------------------------------------------------------|
| `-Name`           | Specifies the name of the web application to retrieve.   |
| `-Site`           | Specifies the name of the IIS site containing the app.   |
| `-ErrorVariable`  | Captures errors to a specified variable.                 |
| `-ErrorAction`    | Determines behavior when errors occur (e.g., `Stop`).    |

## Usage Examples

### Retrieve All Web Applications

```powershell
Get-WebApplication
```

### Retrieve a Specific Web Application by Name

```powershell
Get-WebApplication -Name "MyWebApp"
```

### Retrieve Web Applications for a Specific Site

```powershell
Get-WebApplication -Site "Default Web Site"
```

### Capture Errors in a Variable

```powershell
Get-WebApplication -Name "NonExistentApp" -ErrorVariable appError
```

## Cheat Sheet

```plaintext
Get-WebApplication                  # List all web applications
Get-WebApplication -Name "AppName"  # Get specific web app by name
Get-WebApplication -Site "SiteName" # Get apps for a specific site
```
