# Get-Website Command

`Get-Website` is a PowerShell command used to retrieve information about websites configured in the Internet Information Services (IIS) on a Windows server.

## Common Options

| Option             | Explanation                                    |
|--------------------|------------------------------------------------|
| `-Name`            | Specifies the name of the website to retrieve. |
| `-Server`          | Designates the server from which to get info.  |
| `-Filter`          | Allows filtering of results using criteria.    |

## Usage Examples

### List All Websites
```powershell
Get-Website
```

### Get a Specific Website by Name
```powershell
Get-Website -Name "MyWebsite"
```

### Filter Websites by State
```powershell
Get-Website | Where-Object { $_.State -eq 'Started' }
```

## Cheat Sheet

- **List all websites:**
  ```powershell
  Get-Website
  ```
- **Get site by name:**
  ```powershell
  Get-Website -Name "SiteName"
  ```
- **Filter by state:**
  ```powershell
  Get-Website | Where-Object { $_.State -eq 'Started' }
  ```
