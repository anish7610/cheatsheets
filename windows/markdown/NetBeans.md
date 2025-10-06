# NetBeans Command Overview

The `NetBeans` command is used to launch the NetBeans Integrated Development Environment (IDE) from the command line. It is primarily used by developers to start the IDE with specific parameters or configurations.

## Common Options

| Command           | Description                                                |
|-------------------|------------------------------------------------------------|
| `--userdir <dir>` | Specifies the user directory for NetBeans configuration.   |
| `--cachedir <dir>`| Sets the cache directory for NetBeans.                     |
| `--fontsize <size>`| Sets the font size for the IDE.                           |
| `--jdkhome <dir>` | Specifies the JDK installation directory for NetBeans.     |
| `--nosplash`      | Disables the splash screen on startup.                     |
| `--locale <lang>` | Sets the locale for NetBeans.                              |
| `--help`          | Displays help information for available options.           |

## Usage Examples

### Launch NetBeans with a Specific User Directory

```bash
NetBeans --userdir /path/to/userdir
```

### Start NetBeans Without a Splash Screen

```bash
NetBeans --nosplash
```

### Set Custom Font Size

```bash
NetBeans --fontsize 14
```

### Specify JDK Home Directory

```bash
NetBeans --jdkhome /path/to/jdk
```

## Cheat Sheet

```
NetBeans --userdir <dir>
NetBeans --nosplash
NetBeans --fontsize <size>
NetBeans --jdkhome <dir>
NetBeans --cachedir <dir>
NetBeans --locale <lang>
```

Use these commands to quickly configure and launch NetBeans as needed.
