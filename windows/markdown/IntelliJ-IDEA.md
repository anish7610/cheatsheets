# `IntelliJ IDEA` Command Line Tool

The `IntelliJ IDEA` command is used to open projects from the command line using IntelliJ IDEA, a popular Integrated Development Environment (IDE) for Java and other languages. It allows users to start the IDE, open specific files, and perform other IntelliJ functions directly from the terminal.

## Common Options

| Option     | Description                                              |
|------------|----------------------------------------------------------|
| `-h` or `--help` | Displays help information for the command.           |
| `project_path` | Opens the specified project in IntelliJ IDEA.         |
| `file_path`   | Opens the specified file in IntelliJ IDEA.             |
| `-p` or `--project` | Specifies the project directory to open.          |
| `-e` or `--line` | Opens a specific file at a specified line number.    |

## Usage Examples

### Open a Project

```bash
idea /path/to/your/project
```

### Open a Specific File

```bash
idea /path/to/your/file.java
```

### Open a File at a Specific Line

```bash
idea -e 42 /path/to/your/file.java
```

### Open IntelliJ with Help Information

```bash
idea --help
```

## Cheat Sheet

```plaintext
idea [OPTIONS] [project_path | file_path]
  -h, --help           Show help information
  -p, --project        Open project directory
  -e, --line NUM       Open file at line number
```
