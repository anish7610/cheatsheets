# DBeaver Command

`dbeaver` is a free, multi-platform database management tool that supports various database systems like MySQL, PostgreSQL, Oracle, and others. It provides a graphical interface for database operations including querying, editing, and data visualization.

## Common Options

| Option                | Explanation                               |
|-----------------------|-------------------------------------------|
| `-con <name>`         | Connects to a specified database profile. |
| `-data <workspace>`   | Specifies the path to the workspace.      |
| `-nosplash`           | Starts DBeaver without the splash screen. |
| `-debug`              | Starts DBeaver in debug mode.             |
| `-vmargs`             | Passes arguments directly to JVM.         |

## Usage Examples

### Connect to a Database Profile

Run DBeaver and connect immediately to a database profile:

```bash
dbeaver -con mydatabase
```

### Specify Workspace

Start DBeaver with a specific workspace directory:

```bash
dbeaver -data /path/to/workspace
```

### Start Without Splash Screen

```bash
dbeaver -nosplash
```

### Debug Mode

Start DBeaver in debug mode to assist with troubleshooting:

```bash
dbeaver -debug
```

## Cheat Sheet

```plaintext
dbeaver -con <name>       # Connect to a database profile
dbeaver -data <workspace> # Specify workspace
dbeaver -nosplash         # No splash screen
dbeaver -debug            # Debug mode
```
