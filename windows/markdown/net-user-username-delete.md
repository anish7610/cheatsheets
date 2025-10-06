# `net user [username] /delete`

## Description

This Windows command is used to delete a user account on a local or remote system. It requires administrative privileges to execute.

## Common Options

| Option               | Description                             |
|----------------------|-----------------------------------------|
| `[username]`         | Specifies the name of the user account to delete. |
| `/domain`            | Performs the operation on a domain controller. |

## Usage Examples

### Delete a Local User Account
```shell
net user johndoe /delete
```

### Delete a Domain User Account
```shell
net user janedoe /delete /domain
```

## Cheat Sheet

```markdown
# Delete a local user
net user [username] /delete

# Delete a user on a domain
net user [username] /delete /domain
```
