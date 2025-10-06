# Get-PackageSource Command

`Get-PackageSource` is a Windows PowerShell command used to retrieve information about available package sources (repositories) for package management. It is part of the `PackageManagement` module.

## Common Options

| Option          | Description                                                            |
|-----------------|------------------------------------------------------------------------|
| `-Name`         | Specifies the name of the package source to retrieve.                  |
| `-ProviderName` | Specifies the package provider, such as `NuGet` or `msi`.              |
| `-Location`     | Filters the package sources by their location URL.                     |
| `-Trusted`      | Limits the results to sources marked as trusted.                       |
| `-AllVersions`  | Retrieves all versions of the package sources.                         |
| `-Credential`   | Specifies credentials to access the package source if authentication is required. |

## Usage Examples

### List All Package Sources

```powershell
Get-PackageSource
```

### Retrieve a Specific Package Source by Name

```powershell
Get-PackageSource -Name "MyPackageSource"
```

### List Package Sources for a Specific Provider

```powershell
Get-PackageSource -ProviderName "NuGet"
```

### List Trusted Package Sources

```powershell
Get-PackageSource -Trusted
```

## Cheat Sheet

```plaintext
# List all package sources
Get-PackageSource

# Get package source by name
Get-PackageSource -Name "<SourceName>"

# Get sources by provider
Get-PackageSource -ProviderName "<ProviderName>"

# List only trusted sources
Get-PackageSource -Trusted
```
