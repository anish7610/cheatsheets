# `setfacl` Command in Linux

The `setfacl` command is used in Linux to set file access control lists (ACLs), allowing more flexible permissions than the traditional user/group/other system. This is especially useful for setting permissions for multiple users or groups on a single file or directory.

## Common Options

| Option      | Explanation                                                                 |
|-------------|-----------------------------------------------------------------------------|
| `-m`        | Modify the ACL of a file or directory.                                      |
| `-x`        | Remove specific entries from the ACL.                                       |
| `-b`        | Remove all ACL entries (except the base entries).                           |
| `-k`        | Remove the default ACL.                                                     |
| `-R`        | Apply changes recursively to all files and directories.                     |
| `-d`        | Set the default ACL for directories (affects new files within the directory).|
| `--set`     | Replace the current ACL with the specified one.                             |
| `-L`        | Follow symbolic links when setting or modifying ACLs.                       |
| `-n`        | Do not recalculate the effective rights mask.                               |

## Usage Examples

### Set ACL for a User
Set read and write permissions for user `alice` on `file.txt`:

```bash
setfacl -m u:alice:rw file.txt
```

### Remove ACL for a User
Remove the ACL entry for user `bob` on `file.txt`:

```bash
setfacl -x u:bob file.txt
```

### Set Default ACL for a Directory
Set default permissions for user `carol` on a directory `docs`, affecting new files:

```bash
setfacl -d -m u:carol:rw docs
```

### Apply Changes Recursively
Give group `developers` read and execute permissions on a directory `project` and all its files:

```bash
setfacl -R -m g:developers:rx project
```

### Remove All ACL Entries
Clear all ACL entries from `file.txt`:

```bash
setfacl -b file.txt
```

## Cheat Sheet

```plaintext
# Set ACL for a user
setfacl -m u:user:permissions file

# Remove ACL for a user
setfacl -x u:user file

# Set default ACL for a directory
setfacl -d -m u:user:permissions directory

# Recursively set ACL for a group
setfacl -R -m g:group:permissions directory

# Remove all ACL entries
setfacl -b file
```
