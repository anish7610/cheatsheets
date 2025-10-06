# `icacls` Command

`icacls` is a command-line utility in Windows used to modify and display access control lists (ACLs) on files and directories. It helps manage permissions and inheritance, providing a more flexible way than older tools like `cacls`.

## Common Options

| Option                   | Description                                                                                                        |
|--------------------------|--------------------------------------------------------------------------------------------------------------------|
| `/grant`                 | Grants specified user access rights to a file or directory.                                                        |
| `/deny`                  | Denies specified user access rights, overriding previous grants.                                                   |
| `/remove`                | Removes all occurrences of specified user’s permission.                                                            |
| `/inheritance`           | Changes the inheritance settings for a file or directory.                                                          |
| `/setowner`              | Changes the owner of a file or directory.                                                                           |
| `/findsid`               | Finds and displays ACLs that contain the specified security identifier (SID).                                       |
| `/verify`                | Finds files with ACLs that are potentially corrupted or inconsistent.                                              |
| `/t`                     | Applies the operation to all specified files in the current directory and its subdirectories.                      |
| `/q`                     | Suppresses success messages.                                                                                       |
| `/c`                     | Continues the operation despite errors.                                                                             |
| `/backup`                | Stores the current ACLs of files and directories to a file.                                                        |
| `/restore`               | Restores ACLs stored in a file during a previous backup operation.                                                 |

## Usage Examples

### Grant Full Control to a User

```shell
icacls "C:\example\file.txt" /grant John:F
```

### Deny Write Access to a User

```shell
icacls "C:\example\file.txt" /deny John:W
```

### Remove a User from ACL

```shell
icacls "C:\example\file.txt" /remove John
```

### Change Ownership

```shell
icacls "C:\example\file.txt" /setowner Administrator
```

### Apply Changes Recursively

```shell
icacls "C:\example" /grant John:(OI)(CI)F /t
```

### Backup ACLs

```shell
icacls "C:\example" /save acl_backup.txt /t
```

### Restore ACLs

```shell
icacls "C:\example" /restore acl_backup.txt
```

## Cheat Sheet

```plaintext
# Grant full control
icacls "path" /grant User:F

# Deny write access
icacls "path" /deny User:W

# Remove user access
icacls "path" /remove User

# Change owner
icacls "path" /setowner User

# Recursive apply
icacls "path" /grant User:(OI)(CI)F /t

# Backup
icacls "path" /save file.txt /t

# Restore
icacls "path" /restore file.txt
```
