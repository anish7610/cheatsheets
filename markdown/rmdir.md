# `rmdir` Command in Linux

The `rmdir` command is used to remove empty directories in Linux. It's a straightforward way to clean up directory structures that are no longer needed.

## Common Options

| Option     | Explanation                                                    |
|------------|----------------------------------------------------------------|
| `--ignore-fail-on-non-empty` | Prevents error messages for non-empty directories.  |
| `-p`       | Remove DIRECTORY and its parent directories if they are empty. |

## Usage Examples

### Remove a Single Directory
To remove an empty directory named `example`:
```bash
rmdir example
```

### Remove a Directory Tree
To remove a directory and parent directories if empty:
```bash
rmdir -p example/parent/child
```

### Ignore Fail on Non-Empty
To attempt removal without error messages for non-empty directories:
```bash
rmdir --ignore-fail-on-non-empty example
```

## Cheat Sheet

```plaintext
# Remove an empty directory
rmdir <directory>

# Remove a directory and its ancestors if they become empty
rmdir -p <dir_path>

# Silent removal ignoring errors for non-empty dirs
rmdir --ignore-fail-on-non-empty <directory>
```
