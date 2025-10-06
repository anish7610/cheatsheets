# `whoami /groups`

The `whoami /groups` command in Windows displays the user groups to which the current user belongs. It offers a detailed view of group memberships, indicating each group's security identifier (SID) and attributes.

## Common Options

| Option       | Description                                             |
|--------------|---------------------------------------------------------|
| `/groups`    | Lists all groups the user is a member of, with details. |
| `/fo LIST`   | Formats the output as a list (default format).          |
| `/fo TABLE`  | Formats the output in a table layout.                   |
| `/fo CSV`    | Formats the output in CSV format.                       |

## Usage Examples

### Example 1: Basic Group Information

```cmd
whoami /groups
```

This command lists all the groups to which the current user belongs, including domain and local groups.

### Example 2: Format Output as a Table

```cmd
whoami /groups /fo TABLE
```

Formats the group information in a readable table format.

### Example 3: Export Group Information to CSV

```cmd
whoami /groups /fo CSV > groups.csv
```

Saves the group information in CSV format to a file named `groups.csv`.

## Cheat Sheet

```plaintext
# List your group memberships
whoami /groups

# Table format
whoami /groups /fo TABLE

# CSV format
whoami /groups /fo CSV > groups.csv
```
