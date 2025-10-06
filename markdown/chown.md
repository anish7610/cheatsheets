# `chown` Command in Linux

The `chown` command in Linux is used to change the ownership of files and directories, allowing users to modify which user or group has access permissions.

## Common Options

| Option         | Description                                        |
|----------------|----------------------------------------------------|
| `--recursive`  | Recursively change ownership for directories and their contents. |
| `--verbose`    | Display a message for each file processed.         |
| `--reference`  | Change the ownership to match that of a reference file. |
| `-f, --silent` | Suppress most error messages.                      |

## Usage Examples

1. **Change Owner of a File**
   Change the owner of `file.txt` to `newuser`.
   ```bash
   chown newuser file.txt
   ```

2. **Change Owner and Group of a File**
   Change the owner to `newuser` and the group to `newgroup`.
   ```bash
   chown newuser:newgroup file.txt
   ```

3. **Recursive Change**
   Change the owner of all files in `dir` and its subdirectories.
   ```bash
   chown -R newuser dir/
   ```

4. **Verbose Output**
   View details of ownership changes.
   ```bash
   chown --verbose newuser:newgroup file.txt
   ```

5. **Match Ownership of a Reference File**
   Change ownership to match `reference.txt`.
   ```bash
   chown --reference=reference.txt targetfile.txt
   ```

## Cheat Sheet

```bash
chown [OPTIONS] OWNER[:GROUP] FILE...
chown newuser file.txt
chown newuser:newgroup file.txt
chown -R newuser dir/
chown --verbose newuser file.txt
```
