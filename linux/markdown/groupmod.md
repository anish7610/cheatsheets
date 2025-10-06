# `groupmod` Command

`groupmod` is used to modify existing group definitions on a Linux system. It allows you to change the group name, GID, and other attributes.

## Common Options

| Option   | Description                                 |
|----------|---------------------------------------------|
| `-g`     | Change the Group ID (GID) of the group.     |
| `-n`     | Change the name of the group.               |
| `-o`     | Allow the use of a duplicate GID.           |

## Usage Examples

### Change Group Name

```bash
sudo groupmod -n newgroupname oldgroupname
```
*Changes the group name from `oldgroupname` to `newgroupname`.*

### Change Group GID

```bash
sudo groupmod -g 1001 groupname
```
*Changes the GID of `groupname` to `1001`.*

### Allow Duplicate GID

```bash
sudo groupmod -o -g 1001 groupname
```
*Changes the GID to `1001`, allowing duplicates.*

## Cheat Sheet

```plaintext
# Change group name
sudo groupmod -n NEW_NAME OLD_NAME

# Change group GID
sudo groupmod -g NEW_GID GROUP_NAME

# Allow duplicate GID when changing
sudo groupmod -o -g DUPLICATE_GID GROUP_NAME
```
