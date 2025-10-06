## `net localgroup [groupname] [username] /delete`

### Description

`net localgroup [groupname] [username] /delete` is a Windows command used to remove a user from a specific local group on a machine. This command helps manage group memberships on a local computer.

### Common Options

| Option    | Description                                 |
|-----------|---------------------------------------------|
| `[groupname]` | The name of the local group to modify.        |
| `[username]`  | The name of the user to remove from the group.|
| `/delete` | Removes the specified user from the group.   |

### Examples

#### Remove a User from the Administrators Group

```bash
net localgroup Administrators Alice /delete
```

#### Remove a User from the Users Group

```bash
net localgroup Users Bob /delete
```

#### Remove a User from a Custom Group

Assuming there's a custom group named "Developers":

```bash
net localgroup Developers Carol /delete
```

### Cheat Sheet

```plaintext
# General Syntax
net localgroup [groupname] [username] /delete

# Examples
net localgroup Administrators Alice /delete
net localgroup Users Bob /delete
net localgroup Developers Carol /delete
```
