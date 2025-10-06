# Rider Command in Windows

The `Rider` command is used to launch the JetBrains Rider IDE, a powerful development environment for .NET, ASP.NET, and Unity projects.

## Common Options

| Option             | Description                                          |
|--------------------|------------------------------------------------------|
| `--help`           | Display help information.                            |
| `--version`        | Display the version of Rider.                        |
| `project-file`     | Opens a specified project file in Rider.             |
| `--line <number>`  | Opens a file at a specific line number.              |
| `--disable-plugins`| Launch without loading any plugins.                  |
| `--headless`       | Start Rider in headless mode, useful for automation. |

## Usage Examples

### Open a Project

```sh
Rider MyProject.sln
```

### Open a File at a Specific Line

```sh
Rider --line 42 MyFile.cs
```

### Launch Rider Without Plugins

```sh
Rider --disable-plugins
```

## Cheat Sheet

```plaintext
# Open project
Rider <project-file>

# Open specific file/line
Rider --line <number> <file-path>

# Launch without plugins
Rider --disable-plugins

# Show version
Rider --version

# Help
Rider --help
```
