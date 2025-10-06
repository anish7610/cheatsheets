# `Get-Package` Command in Windows

## Description
`Get-Package` is a command used in Windows PowerShell to list software packages installed on a system. It provides details about each package, allowing users to manage their software inventory effectively.

## Common Options

| Option          | Description                                           |
|-----------------|-------------------------------------------------------|
| `-Name`         | Filters packages by name.                            |
| `-ProviderName` | Specifies the package provider (e.g., MSI, NuGet).    |
| `-AllVersions`  | Lists all available versions of a package.            |
| `-Source`       | Specifies the source of the package (e.g., a URL).    |
| `-Scope`        | Filters packages by scope (e.g., AllUsers, CurrentUser).|

## Usage Examples

### List All Installed Packages
```powershell
Get-Package
```

### Filter Packages by Name
```powershell
Get-Package -Name "Microsoft Office"
```

### List Packages with Specific Provider
```powershell
Get-Package -ProviderName "MSI"
```

### Display All Versions of a Package
```powershell
Get-Package -Name "PackageName" -AllVersions
```

### List Packages for Current User
```powershell
Get-Package -Scope CurrentUser
```

## Cheat Sheet

```plaintext
# List all packages
Get-Package

# Filter by name
Get-Package -Name "<PackageName>"

# Use specific provider
Get-Package -ProviderName "<ProviderName>"

# Show all versions
Get-Package -Name "<PackageName>" -AllVersions

# Filter by user scope
Get-Package -Scope CurrentUser
```

By using these options and examples, you can efficiently manage packages on a Windows system using PowerShell's `Get-Package` command.
