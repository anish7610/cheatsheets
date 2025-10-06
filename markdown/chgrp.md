# `chgrp` Command in Linux

The `chgrp` command in Linux is used to change the group ownership of files or directories.

## Common Options

| Option | Description                                   |
|--------|-----------------------------------------------|
| `-R`   | Recursively change group ownership.           |
| `-v`   | Verbosely describe the action for each file.  |
| `-c`   | Like `-v`, but only reports when a change is made. |
| `--reference=RFILE` | Use RFILE's group instead of specifying a group. |

## Usage Examples

1. **Basic Group Change:**

   ```bash
   chgrp newgroup filename.txt
   ```

2. **Recursively Change Group Ownership:**

   ```bash
   chgrp -R newgroup /path/to/directory
   ```

3. **Verbose Output:**

   ```bash
   chgrp -v newgroup filename.txt
   ```

4. **Change to Group of Reference File:**

   ```bash
   chgrp --reference=ref.txt file.txt
   ```

5. **Change and Print Only When Changed:**

   ```bash
   chgrp -c newgroup file.txt
   ```

## Cheat Sheet

```plaintext
# Change group ownership
chgrp [OPTION]... GROUP FILE...

# Change group ownership recursively
chgrp -R GROUP DIRECTORY

# Verbose and conditional verbose
chgrp -v | -c GROUP FILE
```
