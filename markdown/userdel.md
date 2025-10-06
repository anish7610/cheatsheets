# `userdel` Command in Linux

The `userdel` command is used to delete a user account and related files from a Linux system.

## Common Options

| Option    | Explanation                                                    |
|-----------|----------------------------------------------------------------|
| `-r`      | Remove the user's home directory and mail spool                |
| `-f`      | Force the removal of the user, even if they are logged in      |

## Usage Examples

### Delete a User Account
```bash
sudo userdel username
```

### Delete a User Account and Home Directory
```bash
sudo userdel -r username
```

### Forcibly Delete a User Currently Logged In
```bash
sudo userdel -f username
```

## Cheat Sheet

```
# Delete a user
sudo userdel username

# Delete a user and their home directory
sudo userdel -r username

# Force delete a user currently logged in
sudo userdel -f username
```

Ensure you have administrative privileges to execute these commands and exercise caution, especially with the `-r` and `-f` options, to avoid accidental data loss.
