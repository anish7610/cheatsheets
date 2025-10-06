### Description

`Remove-LocalGroupMember` is a PowerShell cmdlet used to remove users or groups from a local security group on a Windows system. It is useful for managing permissions and access control on a local machine.

### Common Options

| Option                  | Explanation                                               |
|-------------------------|-----------------------------------------------------------|
| `-Group`                | Specifies the name of the local group.                    |
| `-Member`               | Specifies the user or group to remove from the local group. |
| `-Confirm`              | Prompts for confirmation before executing the command.    |
| `-WhatIf`               | Shows what would happen if the command is executed, without making changes. |

### Usage Examples

#### Example 1: Remove a Single User from a Group

```powershell
Remove-LocalGroupMember -Group "Administrators" -Member "JohnDoe"
```

*Removes the user "JohnDoe" from the "Administrators" group.*

#### Example 2: Remove Multiple Users from a Group

```powershell
Remove-LocalGroupMember -Group "Users" -Member "JohnDoe", "JaneSmith"
```

*Removes the users "JohnDoe" and "JaneSmith" from the "Users" group.*

#### Example 3: View Potential Changes with `-WhatIf`

```powershell
Remove-LocalGroupMember -Group "Developers" -Member "DevUser" -WhatIf
```

*Displays what would happen if "DevUser" were removed from the "Developers" group without actually performing the operation.*

#### Example 4: Prompt for Confirmation

```powershell
Remove-LocalGroupMember -Group "Support" -Member "OldUser" -Confirm
```

*Prompts the user for confirmation before removing "OldUser" from the "Support" group.*

### Cheat Sheet

```plaintext
Remove-LocalGroupMember -Group "GroupName" -Member "UserName"
Remove-LocalGroupMember -Group "GroupName" -Member "User1", "User2"
Remove-LocalGroupMember -Group "GroupName" -Member "UserName" -WhatIf
```
