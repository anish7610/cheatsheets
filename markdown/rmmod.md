# `rmmod` Command

The `rmmod` command is used in Linux to remove a module from the Linux kernel. This is part of managing kernel modules dynamically, allowing for unloading when they are no longer needed.

## Common Options

| Option    | Description                                  |
|-----------|----------------------------------------------|
| `-f`      | Force module removal, even if in use.        |
| `-v`      | Verbose mode; provides additional details.   |
| `-w`      | Wait until the module is no longer in use.   |
| `-s`      | Log errors using syslog instead of stderr.   |

## Usage Examples

### Remove a Module

```bash
rmmod my_module
```

### Verbosely Remove a Module

```bash
rmmod -v my_module
```

### Force Remove a Module

```bash
sudo rmmod -f my_module
```

### Wait Until Module Is Not In Use

```bash
sudo rmmod -w my_module
```

## Cheat Sheet

```bash
rmmod [options] <module_name>
```

- **Remove a module:** `rmmod my_module`
- **Verbose mode:** `rmmod -v my_module`
- **Force removal:** `sudo rmmod -f my_module`
- **Wait until free:** `sudo rmmod -w my_module`
