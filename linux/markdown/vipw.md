# `vipw` Command in Linux

`vipw` is used to safely edit the `/etc/passwd` and `/etc/shadow` files. It locks the files to prevent simultaneous edits by other processes or users.

## Common Options

| Option | Description                              |
|--------|------------------------------------------|
| `-g`   | Edit the `/etc/group` file instead.      |
| `-s`   | Edit the `/etc/shadow` file as well.     |

## Usage Examples

### Edit the `/etc/passwd` File

To securely edit the user information:

```bash
sudo vipw
```

### Edit the `/etc/group` File

To edit group information:

```bash
sudo vipw -g
```

### Edit the `/etc/shadow` File

To edit the shadow file (along with the passwd file):

```bash
sudo vipw -s
```

## Cheat Sheet

```bash
sudo vipw      # Edit /etc/passwd
sudo vipw -g   # Edit /etc/group
sudo vipw -s   # Edit /etc/passwd and /etc/shadow
```

Always use `vipw` for atomic operations and file consistency.
