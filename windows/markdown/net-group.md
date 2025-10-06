# `net group` Command

The `net group` command is used in Windows to manage group accounts on local or remote servers. It allows administrators to add, delete, and manage group memberships.

## Common Options

| Option          | Description                                            |
|-----------------|--------------------------------------------------------|
| `/add`          | Creates a new group.                                   |
| `/delete`       | Deletes a group.                                       |
| `/domain`       | Performs the operation on the primary domain controller. |
| `groupname`     | Specifies the name of the group to manage.             |
| `/comment:"text"` | Adds a comment for the group.                        |
| `/members`      | Lists members of a specified group.                    |
| `username /add` | Adds a user to the group.                              |
| `username /delete` | Removes a user from the group.                     |

## Usage Examples

### Create a New Group

```bash
net group Marketing /add
```

### Delete an Existing Group

```bash
net group Marketing /delete
```

### Add a User to a Group

```bash
net group Marketing johndoe /add
```

### Remove a User from a Group

```bash
net group Marketing johndoe /delete
```

### List Members of a Group

```bash
net group Marketing /members
```

### Create a Group with a Comment

```bash
net group Sales /add /comment:"Sales team members"
```

## Cheat Sheet

```bash
# Create group
net group <groupname> /add

# Delete group
net group <groupname> /delete

# Add user to group
net group <groupname> <username> /add

# Remove user from group
net group <groupname> <username> /delete

# List group members
net group <groupname> /members
```
