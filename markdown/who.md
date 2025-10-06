# Linux `who` Command

The `who` command in Linux is used to display information about users who are currently logged into the system.

## Common Options

| Option | Description                                    |
|--------|------------------------------------------------|
| `-H`   | Display the list with headers.                 |
| `-u`   | Include idle time for each user.               |
| `-q`   | Display a quick list of all logged-in users.   |
| `-b`   | Show the last system boot time.                |

## Usage Examples

### Display Logged-in Users with Headers
```bash
who -H
```

### Show Users with Idle Time
```bash
who -u
```

### Quick List of Logged-in Users
```bash
who -q
```

### Last System Boot Time
```bash
who -b
```

## Cheat Sheet

```plaintext
# Display logged-in users with headers
who -H

# Include idle time
who -u

# Quick list of users
who -q

# Last boot time
who -b
```
