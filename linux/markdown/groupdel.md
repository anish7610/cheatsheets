# `groupdel` Command in Linux

The `groupdel` command is used to delete a group from the system. It modifies the `/etc/group` and `/etc/gshadow` files to remove all entries that refer to the specified group.

## Common Options

| Option | Description                        |
|--------|------------------------------------|
| `-h`   | Display help message and exit.     |

## Usage Examples

### Delete a Group

To delete a group named `developers`:

```bash
sudo groupdel developers
```

### Attempt to Delete an In-use Group

The `groupdel` command cannot delete a group if it is the primary group for any existing user. Ensure no users are assigned to the group before deleting.

### Confirm Group Deletion

Check if the group has been deleted:

```bash
getent group | grep developers
```

This should return no output if the group has been successfully deleted.

## Cheat Sheet

```plaintext
# Delete a group
sudo groupdel <groupname>

# Display help message
groupdel -h

# Confirming group deletion
getent group | grep <groupname>
```
