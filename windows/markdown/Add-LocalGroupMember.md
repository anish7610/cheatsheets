# Add-LocalGroupMember Command

`Add-LocalGroupMember` is a Windows PowerShell command used to add users or groups to a local security group on a system. It is commonly used for managing user permissions locally.

## Common Options

| Option                     | Explanation                                              |
|----------------------------|----------------------------------------------------------|
| `-Group`                   | Specifies the name of the local group to modify.         |
| `-Member`                  | Identifies the user or group to add to the local group.  |
| `-WhatIf`                  | Shows what would happen if the command runs, without executing it. |
| `-Confirm`                 | Prompts for confirmation before executing the command.   |

## Usage Examples

### Add a User to a Local Group

```powershell
Add-LocalGroupMember -Group "Administrators" -Member "username"
```

### Add Multiple Users and Groups

```powershell
Add-LocalGroupMember -Group "Administrators" -Member "user1", "user2", "GroupName"
```

### Check the Command without Executing

```powershell
Add-LocalGroupMember -Group "Administrators" -Member "username" -WhatIf
```

### Prompt for Confirmation

```powershell
Add-LocalGroupMember -Group "Users" -Member "username" -Confirm
```

## Cheat Sheet

```plaintext
Add-LocalGroupMember -Group "GroupName" -Member "UserName, GroupName"
```

- **Preview Changes:** `-WhatIf`
- **Confirmation Prompt:** `-Confirm`

Use this command to efficiently manage local group memberships.
