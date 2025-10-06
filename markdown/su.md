# `su` Command in Linux

The `su` (substitute user) command is used to switch to another user account in the current shell session. By default, it switches to the root user.

## Common Options

| Option  | Description                                       |
|---------|---------------------------------------------------|
| `-`     | Start a login shell, reinitializing the environment. |
| `-c`    | Run a single command as a specific user.          |
| `-s`    | Specify a shell to use instead of the default.    |
| `-p`    | Preserve the current environment.                 |

## Usage Examples

### Switch to Root User

```bash
su
```

### Switch to a Specific User

```bash
su username
```

### Switch to Root with a Login Shell

```bash
su -
```

### Run a Command as Another User

```bash
su -c "ls /root" username
```

### Use a Different Shell

```bash
su -s /bin/bash username
```

## Cheat Sheet

```plaintext
su            # Become root
su username   # Switch to specific user
su -          # Switch with login shell
su -c "cmd"   # Run single command
su -s shell   # Use specified shell
```
