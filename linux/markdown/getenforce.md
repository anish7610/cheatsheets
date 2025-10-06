# `getenforce` Command Overview

The `getenforce` command is used in Linux to query the current mode of SELinux (Security-Enhanced Linux). It provides a simple output indicating whether SELinux is enforcing, permissive, or disabled.

## Common Options

| Option | Description                        |
|--------|------------------------------------|
| N/A    | The `getenforce` command has no options. Its sole purpose is to output the current SELinux mode. |

## Usage Examples

### Example 1: Check SELinux Status
```bash
getenforce
```
This will output either `Enforcing`, `Permissive`, or `Disabled`.

### Example 2: Use in a Script to Conditionally Act
```bash
if [ "$(getenforce)" = "Enforcing" ]; then
    echo "SELinux is enforcing. Adjusting settings."
else
    echo "SELinux is not enforcing. No changes needed."
fi
```

## Cheat Sheet

```bash
# Check SELinux mode
getenforce
```

- `Enforcing`: SELinux actively enforces policies.
- `Permissive`: SELinux logs actions that would be blocked.
- `Disabled`: SELinux is turned off.
