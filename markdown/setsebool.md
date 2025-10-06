# `setsebool` Command in Linux

The `setsebool` command is used to manage SELinux boolean values, which allow administrators to enable or disable certain SELinux policy features without loading a new policy.

## Common Options

| Option           | Explanation                                                             |
|------------------|-------------------------------------------------------------------------|
| `-P`             | Makes the change persistent across reboots.                             |
| `-N`             | Do not execute the command but show what would be done.                 |
| `-V`             | Verbosely display the changes being made.                               |

## Usage Examples

### Temporarily Enable a Boolean

Enable HTTPD to read home directories:

```bash
setsebool httpd_read_user_content on
```

### Permanently Enable a Boolean

Enable Samba to export home directories:

```bash
setsebool -P samba_export_all_rw on
```

### Verbose Output

Enable NFS for confined processes and show verbose output:

```bash
setsebool -V allow_nfsd_anon_write on
```

## Cheat Sheet

```bash
# Temporarily change a SELinux boolean
setsebool <boolean_name> on|off

# Permanently change a SELinux boolean
setsebool -P <boolean_name> on|off

# Verbose output
setsebool -V <boolean_name> on|off
```

Replace `<boolean_name>` with the actual boolean you wish to modify.
