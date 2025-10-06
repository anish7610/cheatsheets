## Remove-Module Command

`Remove-Module` is a PowerShell command used to remove modules from the current session in Windows. This can help free up resources or ensure that specific versions are unloaded.

### Common Options

| Option              | Description                                                     |
|---------------------|-----------------------------------------------------------------|
| `-Name`             | Specifies the name of the module to remove.                     |
| `-FullyQualifiedName` | Removes a module using its fully qualified name.              |
| `-ErrorAction`      | Determines how the command responds to non-terminating errors.  |
| `-Force`            | Forces removal of a module even if it is in use.                |
| `-Verbose`          | Provides detailed information about the operation.              |

### Usage Examples

#### Remove a Module by Name
```powershell
Remove-Module -Name "ModuleName"
```

#### Force Removal of a Module
```powershell
Remove-Module -Name "ModuleName" -Force
```

#### Remove a Module with Detailed Output
```powershell
Remove-Module -Name "ModuleName" -Verbose
```

### Cheat Sheet

```plaintext
# Remove a module by name
Remove-Module -Name "ModuleName"

# Force removal of the module
Remove-Module -Name "ModuleName" -Force

# Remove with detailed information
Remove-Module -Name "ModuleName" -Verbose
```

This succinct format should serve as a quick reference for using `Remove-Module` effectively in various scenarios.
