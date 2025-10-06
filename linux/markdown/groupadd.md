# `groupadd` Command Overview

The `groupadd` command in Linux is used to create new groups on the system. It modifies the `/etc/group` file to add entries for new groups.

## Common Options

| Option       | Description                                    |
|--------------|------------------------------------------------|
| `-f, --force`| Exit successfully if the specified group already exists. |
| `-g, --gid`  | Set the numeric value of the group ID.         |
| `-K, --key`  | Override `/etc/login.defs` settings.           |
| `-o, --non-unique` | Allow creation of groups with duplicate GIDs. |
| `-p, --password` | Specify an encrypted password for the group. |

## Usage Examples

### Create a New Group
Create a group named `developers`:
```bash
sudo groupadd developers
```

### Create a Group with a Specific GID
Create a group named `admins` with GID 1050:
```bash
sudo groupadd -g 1050 admins
```

### Create a Group Allowing Duplicate GIDs
Create a group `testgroup` with non-unique GID 1001:
```bash
sudo groupadd -o -g 1001 testgroup
```

## Cheat Sheet

```plaintext
# Basic group creation
sudo groupadd <groupname>

# Create a group with specific GID
sudo groupadd -g <GID> <groupname>

# Allow duplicate GID
sudo groupadd -o -g <GID> <groupname>
```
