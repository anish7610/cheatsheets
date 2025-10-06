### Description

The command `Get-LocalGroup | Where-Object { $_.Name -eq "Administrators" }` is used in PowerShell to list local groups and filter out the "Administrators" group. It utilizes `Get-LocalGroup` to retrieve all local groups and `Where-Object` to apply a filter based on the group's name.

### Common Options

| Option                   | Explanation                                 |
|--------------------------|---------------------------------------------|
| `-Name`                  | Specifies the name of the local group.      |
| `Where-Object {}`        | Applies a condition to filter objects.      |

### Examples

#### 1. List All Local Groups

```bash
Get-LocalGroup
```

#### 2. Filter the Administrators Group

```bash
Get-LocalGroup | Where-Object { $_.Name -eq "Administrators" }
```

#### 3. Check If a User Is in Administrators Group

```bash
Get-LocalGroupMember -Group "Administrators" | Where-Object { $_.Name -eq "specificuser" }
```

### Cheat Sheet

```bash
# List all local groups
Get-LocalGroup

# Filter Administrators group
Get-LocalGroup | Where-Object { $_.Name -eq "Administrators" }

# Check user in Administrators group
Get-LocalGroupMember -Group "Administrators" | Where-Object { $_.Name -eq "username" }
```
