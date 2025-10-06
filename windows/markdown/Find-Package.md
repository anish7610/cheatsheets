# Find-Package Command in Windows

`Find-Package` is a PowerShell command used to discover packages available through package management providers such as NuGet, PowerShell Gallery, and Chocolatey.

## Common Options

| Option            | Explanation                                                    |
|-------------------|----------------------------------------------------------------|
| `-Name`           | Specifies the name of the package to find.                     |
| `-ProviderName`   | Filters search to a specific provider like `NuGet` or `Choco`. |
| `-Source`         | Specifies a particular source or repository to search.         |
| `-AllVersions`    | Finds all available versions of a package.                     |
| `-RequiredVersion`| Finds a specific version of a package.                         |
| `-IncludeDependencies` | Includes package dependencies in the search result.      |
| `-Credential`     | Uses specific credentials to access the package source.        |

## Usage Examples

### Find a Specific Package

```powershell
Find-Package -Name "git"
```

### Find All Versions of a Package

```powershell
Find-Package -Name "git" -AllVersions
```

### Search for Packages with a Specific Provider

```powershell
Find-Package -ProviderName "NuGet" -Name "Newtonsoft.Json"
```

### Find a Package from a Specific Source

```powershell
Find-Package -Source "https://www.nuget.org/api/v2" -Name "EntityFramework"
```

### Find a Package with Dependencies

```powershell
Find-Package -Name "mypackage" -IncludeDependencies
```

## Cheat Sheet

```plaintext
# Basic search
Find-Package -Name "package-name"

# All versions
Find-Package -Name "package-name" -AllVersions

# Specific provider
Find-Package -ProviderName "provider-name" -Name "package-name"

# Specific source
Find-Package -Source "source-url" -Name "package-name"

# Include dependencies
Find-Package -Name "package-name" -IncludeDependencies
```
