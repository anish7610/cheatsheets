## `Add-PackageSource` Command Overview

`Add-PackageSource` is a Windows PowerShell command that adds a new package source to a computer. It is commonly used to register repositories where packages can be found and installed with package management tools.

### Common Options

| Option            | Description                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| `-Name`           | Specifies the name of the package source.                                   |
| `-Location`       | Defines the URL or file path of the package source.                         |
| `-ProviderName`   | Specifies the package provider (e.g., NuGet, PowerShellGet).                |
| `-Credential`     | Provides a user credential for the source, if authentication is required.   |
| `-Trusted`        | Marks the package source as trusted.                                        |
| `-Force`          | Forces the action without prompting for confirmation.                       |

### Usage Examples

#### Add a NuGet Package Source

```powershell
Add-PackageSource -Name "MyNuGetSource" -Location "https://api.nuget.org/v3/index.json" -ProviderName "NuGet" -Trusted
```

#### Add a PowerShell Gallery Source with Credentials

```powershell
$cred = Get-Credential
Add-PackageSource -Name "MyPSGallery" -Location "https://www.powershellgallery.com/api/v2" -ProviderName "PowerShellGet" -Credential $cred
```

#### Add a Local Package Source

```powershell
Add-PackageSource -Name "LocalRepo" -Location "C:\LocalPackages" -ProviderName "NuGet"
```

### Cheat Sheet

```plaintext
Add-PackageSource -Name <SourceName> -Location <SourceURL/Path> -ProviderName <Provider> [-Credential <Cred>] [-Trusted] [-Force]
```

Use this command to register new package sources for easy package management in your Windows environment.
