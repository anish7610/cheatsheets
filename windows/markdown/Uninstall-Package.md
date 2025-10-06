# Uninstall-Package Command

`Uninstall-Package` is a PowerShell cmdlet used to remove installed packages from a Windows system. It is part of the `PackageManagement` module, which enables software discovery, installation, and inventory.

## Common Options

| Option            | Description                                           |
|-------------------|-------------------------------------------------------|
| `-Name`           | Specifies the name of the package to uninstall.       |
| `-ProviderName`   | Specifies the package provider (e.g., `NuGet`).       |
| `-Force`          | Forces the uninstallation without user confirmation.  |
| `-WhatIf`         | Shows what would happen if the command runs.          |
| `-Verbose`        | Provides detailed information during execution.       |

## Usage Examples

### Uninstall a Package by Name

```powershell
Uninstall-Package -Name "PackageName"
```

### Uninstall a Package Using a Specific Provider

```powershell
Uninstall-Package -Name "PackageName" -ProviderName "NuGet"
```

### Uninstall a Package with Confirmation

```powershell
Uninstall-Package -Name "PackageName" -Force
```

### Preview Uninstallation Without Executing

```powershell
Uninstall-Package -Name "PackageName" -WhatIf
```

### Verbose Output

```powershell
Uninstall-Package -Name "PackageName" -Verbose
```

## Cheat Sheet

```plaintext
Uninstall-Package -Name [PackageName]
Uninstall-Package -Name [PackageName] -ProviderName [Provider]
Uninstall-Package -Name [PackageName] -Force
Uninstall-Package -Name [PackageName] -WhatIf
```

This cheat sheet and the examples provide quick guidance for using `Uninstall-Package` effectively.
