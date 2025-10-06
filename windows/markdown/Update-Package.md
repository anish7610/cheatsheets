# Update-Package Command in Windows

`Update-Package` is a PowerShell command used to update packages in a project, typically within the NuGet package ecosystem. It helps ensure that your project uses the latest versions of dependencies.

## Common Options

| Option                   | Description                                               |
|--------------------------|-----------------------------------------------------------|
| `-Id <string>`           | Specifies the package ID to update.                       |
| `-ProjectName <string>`  | Updates packages in the specified project only.           |
| `-Reinstall`             | Reinstalls the same version of the currently installed package. |
| `-Safe`                  | Updates to the highest version within the same feature band. |
| `-Source <string>`       | Specifies the package source to search.                   |
| `-WhatIf`                | Shows what would happen if the command is executed without making changes. |

## Usage Examples

### Update a Specific Package

```shell
Update-Package -Id 'Newtonsoft.Json'
```

### Update All Packages in a Specific Project

```shell
Update-Package -ProjectName 'MyProject'
```

### Update All Packages Using a Specific Source

```shell
Update-Package -Source 'https://nuget.org/api/v2'
```

### Safe Update to Highest Compatible Version

```shell
Update-Package -Id 'EntityFramework' -Safe
```

## Cheat Sheet

- **Update a Package:** `Update-Package -Id 'PackageName'`
- **Update in a Project:** `Update-Package -ProjectName 'ProjectName'`
- **Reinstall Package:** `Update-Package -Id 'PackageName' -Reinstall`
- **Preview Update:** `Update-Package -Id 'PackageName' -WhatIf`
