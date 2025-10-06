# `passwd` Command Overview

The `passwd` command in Linux is used to update a user's authentication tokens (passwords). It can also lock, unlock, or update account information.

## Common Options

| Option       | Description                                         |
|--------------|-----------------------------------------------------|
| `-d`         | Delete a user's password, allowing passwordless login (not recommended).   |
| `-e`         | Expire a user's password immediately, forcing a password change at next login. |
| `-l`         | Lock a user's account.                              |
| `-u`         | Unlock a user's account.                            |
| `-S`         | Display account status information.                 |
| `--stdin`    | Update password using standard input.               |

## Usage Examples

### Change Your Own Password

```bash
passwd
```

### Change Another User's Password (superuser required)

```bash
sudo passwd username
```

### Lock a User's Account

```bash
sudo passwd -l username
```

### Unlock a User's Account

```bash
sudo passwd -u username
```

### Force Password Change at Next Login

```bash
sudo passwd -e username
```

### Check Account Status

```bash
passwd -S username
```

## Cheat Sheet

```plaintext
# Change your password
passwd

# Change another user's password
sudo passwd username

# Lock/unlock a user account
sudo passwd -l username
sudo passwd -u username

# Force a password change at next login
sudo passwd -e username

# Display account status
passwd -S username
```
