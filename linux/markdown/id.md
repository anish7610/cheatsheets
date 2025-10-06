# `id` Command in Linux

## Description

The `id` command displays the real and effective user and group IDs. It is commonly used to identify the current user or the user and group information of another specified user.

## Common Options

| Option    | Explanation                                          |
|-----------|------------------------------------------------------|
| `-u`      | Print only the effective user ID.                    |
| `-g`      | Print only the effective group ID.                   |
| `-G`      | Print all group IDs.                                 |
| `-n`      | Print a name instead of a numeric ID (used with `-u`, `-g`, or `-G`). |
| `-r`      | Print the real ID instead of the effective ID (used with `-u` or `-g`). |

## Usage Examples

### Default Usage

```bash
id
```
Displays the user and group information for the current user.

### Specifying a User

```bash
id username
```
Displays the user and group information for the specified user.

### Getting Only the User ID

```bash
id -u
```
Prints only the effective user ID for the current user.

### Getting Only the Group ID

```bash
id -g
```
Prints only the effective group ID for the current user.

### Getting Group Names

```bash
id -Gn
```
Displays the group names for the current user.

## Cheat Sheet

```plaintext
id          # Full user and group info for current user
id username # Info for specified user
id -u       # User ID
id -g       # Group ID
id -G       # All group IDs
id -un      # User name
id -gn      # Group name
```
