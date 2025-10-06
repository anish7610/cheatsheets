# `net localgroup [groupname] [username] /add`

## Description

The `net localgroup [groupname] [username] /add` command is used in Windows to add a specified user to a local group. Local groups manage user permissions at the local machine level.

## Common Options

| Option       | Explanation                                              |
|--------------|----------------------------------------------------------|
| `[groupname]`| The name of the local group to which the user is added.  |
| `[username]` | The username of the user to be added to the local group. |
| `/add`       | Adds the specified user to the specified local group.    |

## Usage Examples

```bash
# Add user 'john' to the 'Administrators' group
net localgroup Administrators john /add

# Add user 'maria' to the 'Users' group
net localgroup Users maria /add

# Add user 'anna' to the 'Remote Desktop Users' group
net localgroup "Remote Desktop Users" anna /add
```

## Cheat Sheet

```markdown
# Add a user to a local group
net localgroup [groupname] [username] /add
```

Use quotes for group names with spaces.
