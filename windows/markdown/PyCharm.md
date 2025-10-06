# PyCharm Command

The `pycharm` command is used to launch the PyCharm IDE from the command line. It provides various options to configure the startup behavior and open specific files or projects.

## Common Options

| Option          | Explanation                                              |
|-----------------|----------------------------------------------------------|
| `--line <line>` | Open a file at a specific line number.                   |
| `--wait`        | Wait for the PyCharm process to close before returning.  |
| `--disable-plugins` | Start PyCharm with all plugins disabled.             |
| `-h` or `--help` | Show help information for the command.                  |

## Usage Examples

### Open a Specific File

```bash
pycharm myfile.py
```

### Open a File at a Specific Line

```bash
pycharm --line 10 myfile.py
```

### Open a Project and Wait for Closure

```bash
pycharm --wait myproject/
```

### Start PyCharm with All Plugins Disabled

```bash
pycharm --disable-plugins
```

## Cheat Sheet

```bash
# Open file
pycharm <file>

# Open file at line number
pycharm --line <line> <file>

# Wait for PyCharm closure
pycharm --wait <project>

# Disable all plugins
pycharm --disable-plugins
```

Ensure PyCharm's `bin` directory is in your PATH to use these commands directly.
