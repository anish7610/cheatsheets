# `getfacl` Command Overview

`getfacl` is a command-line utility used in Linux to retrieve the Access Control List (ACL) of files and directories. It displays the permissions set for different users and groups, providing more granular control than traditional Unix file permissions.

## Common Options

| Option | Description                                |
|--------|--------------------------------------------|
| `-a`   | Display the effective rights mask.         |
| `-d`   | Show only default ACLs (useful with directories). |
| `-n`   | Display numeric user and group IDs.        |
| `-p`   | Suppress the file name in output.          |
| `-R`   | Recursively apply to all files/directories.|

## Usage Examples

### View ACL of a File
```bash
getfacl filename.txt
```

### View Default ACLs on a Directory
```bash
getfacl -d /path/to/directory
```

### View ACLs with Numeric IDs
```bash
getfacl -n filename.txt
```

### Recursively View ACLs
```bash
getfacl -R /path/to/directory
```

## Cheat Sheet

```plaintext
# View ACL
getfacl file_or_directory

# View ACL with numeric IDs
getfacl -n file_or_directory

# View default ACLs
getfacl -d directory

# Recursively view ACLs
getfacl -R directory
```

Use `getfacl` to understand detailed permissions beyond the basic read, write, and execute permissions, particularly in environments with complex access controls.
