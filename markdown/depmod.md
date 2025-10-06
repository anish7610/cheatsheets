## `depmod` Command Overview

The `depmod` command is used to generate modules' dependency files. It processes a set of modules and creates a file (`modules.dep`) listing the dependencies, which is essential for proper module loading by `modprobe`.

### Common Options

| Option     | Description                                              |
|------------|----------------------------------------------------------|
| `-a`, `--all` | Probe all modules located in the `/lib/modules/$(uname -r)` directory, the default action. |
| `-b`, `--basedir` | Specify an alternate root directory, useful for chroot environments. |
| `-C`, `--config` | Use a specific depmod configuration file.          |
| `-n`, `--dry-run` | Perform a trial run without changing any files.    |
| `-e`, `--errsyms` | Report unresolved symbols.                        |
| `-F`, `--filesyms` | Use a specific System.map file to check for unresolved symbols. |
| `-v`, `--verbose` | Display detailed information about the process.   |

### Usage Examples

1. **Generate Dependencies for Current Kernel:**

   ```bash
   sudo depmod
   ```

2. **Generate Dependencies for a Specific Kernel Version:**

   ```bash
   sudo depmod 5.4.0-42-generic
   ```

3. **Use an Alternate Root Directory:**

   ```bash
   sudo depmod -b /mnt/myroot
   ```

4. **Verbose Output for Troubleshooting:**

   ```bash
   sudo depmod -v
   ```

5. **Dry Run to Check Dependencies Without Applying:**

   ```bash
   depmod -n
   ```

### Cheat Sheet

```plaintext
# Generate dependencies for the running kernel
sudo depmod

# Generate dependencies for a specific kernel version
sudo depmod [kernel-version]

# Use an alternative root directory
sudo depmod -b [directory]

# Verbose output
sudo depmod -v

# Dry run
depmod -n
```
