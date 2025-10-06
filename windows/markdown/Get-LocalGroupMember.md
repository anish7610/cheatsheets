# Get-LocalGroupMember Command

The `Get-LocalGroupMember` command in Windows PowerShell is used to retrieve members of a local security group. It lists users, groups, and other entities that belong to a specified local group.

## Common Options

| Option        | Explanation                                                  |
|---------------|--------------------------------------------------------------|
| `-Group`      | Specifies the name of the local group to retrieve members from. |
| `-Member`     | Retrieves specific group member details.                     |
| `-SID`        | Displays the security identifier for group members.          |
| `-Credential` | Allows running the command with alternate user credentials.  |

## Usage Examples

### List All Members of a Group

To list all members of the "Administrators" group:

```powershell
Get-LocalGroupMember -Group "Administrators"
```

### Display Security Identifiers

To display security identifiers along with user information:

```powershell
Get-LocalGroupMember -Group "Users" -SID
```

### Retrieve Specific Member Details

To get information about a specific member in the "Users" group:

```powershell
Get-LocalGroupMember -Group "Users" -Member "username"
```

## Cheat Sheet

```bash
Get-LocalGroupMember -Group "<GroupName>"
Get-LocalGroupMember -Group "<GroupName>" -SID
```

Replace `<GroupName>` with the name of the group you want to query.
