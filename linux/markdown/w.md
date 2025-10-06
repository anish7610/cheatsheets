# The `w` Command

The `w` command in Linux displays information about the users currently logged in to the system and their activity. It provides details such as login times, terminal lines, remote host, idle times, JCPU, PCPU, and the command each user is executing.

## Common Options

| Option | Description                                             |
|--------|---------------------------------------------------------|
| `-h`   | Suppress the header line in the output.                 |
| `-s`   | Short format. Omits the JCPU and PCPU times.            |
| `-f`   | Toggle printing of the login field.                     |
| `-u`   | Ignore the username field.                              |
| `-V`   | Display version information and exit.                   |

## Usage Examples

### Display Active Users

```bash
w
```

This displays all currently logged-in users and their activities.

### Suppress Header with Short Format

```bash
w -hs
```

Use both `-h` and `-s` to get a concise list without headers or detailed CPU times.

### Exclude Username Field

```bash
w -u
```

Lists active users without the username field.

## Cheat Sheet

```bash
w           # Show all logged-in users
w -h        # No headers
w -s        # Short format
w -f        # Toggle login field
w -u        # Ignore username field
```
