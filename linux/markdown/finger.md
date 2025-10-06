# Linux `finger` Command

The `finger` command is used to display user information on a Linux system. It retrieves details such as the user's real name, home directory, shell, and more.

## Common Options

| Option       | Description                                       |
|--------------|---------------------------------------------------|
| `[user]`     | Displays information about the specified user.    |
| `-l`         | Provides a long format output. Shows detailed info.|
| `[user@host]`| Queries user information on a remote host.        |

## Usage Examples

### Display Information for Current User

```bash
finger
```

### Display Information for a Specific User

```bash
finger alice
```

### Long Format for a Specific User

```bash
finger -l bob
```

### Remote User Information Retrieval

```bash
finger alice@remotehost
```

## Cheat Sheet

```markdown
finger            # Info for all logged-in users
finger user       # Info for specified user
finger -l user    # Detailed info for specified user
finger user@host  # Remote user info
```
