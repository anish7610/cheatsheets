## Install-Package Command Overview

`Install-Package` is a PowerShell cmdlet used to install software packages from an online source or a local package repository. It is part of the PackageManagement module, which allows managing software dependencies and installations on Windows.

## Common Options

| Option              | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| `-Name`             | Specifies the name of the package to install.                               |
| `-ProviderName`     | Defines the package provider (e.g., NuGet, Chocolatey).                     |
| `-Source`           | Specifies the source repository where the package can be found.             |
| `-RequiredVersion`  | Installs a specific version of the package.                                 |
| `-Scope`            | Determines the installation scope (`CurrentUser` or `AllUsers`).            |
| `-Force`            | Forces reinstalling a package even if it is already installed.              |
| `-Credential`       | Provides user credentials for package sources requiring authentication.     |
| `-DestinationPath`  | Specifies the directory where the package should be installed.              |

## Usage Examples

### Install a Package by Name

```powershell
Install-Package -Name "SampleApp"
```

### Install a Specific Version

```powershell
Install-Package -Name "SampleApp" -RequiredVersion "1.0.0"
```

### Use a Specific Provider

```powershell
Install-Package -Name "SampleApp" -ProviderName "Chocolatey"
```

### Install from a Specific Source

```powershell
Install-Package -Name "SampleApp" -Source "https://example.com/repo"
```

### Install for Current User Only

```powershell
Install-Package -Name "SampleApp" -Scope "CurrentUser"
```

### Force Reinstallation

```powershell
Install-Package -Name "SampleApp" -Force
```

## Cheat Sheet

```plaintext
# Basic installation
Install-Package -Name "PackageName"

# Install a specific version
Install-Package -Name "PackageName" -RequiredVersion "x.x.x"

# Install with specific provider
Install-Package -Name "PackageName" -ProviderName "Provider"

# Install from a source
Install-Package -Name "PackageName" -Source "SourceURL"

# Force and scope options
Install-Package -Name "PackageName" -Scope "Scope" -Force
```
