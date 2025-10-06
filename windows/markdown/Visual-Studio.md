# Visual Studio Command

Visual Studio is an integrated development environment (IDE) from Microsoft used for developing applications. Its command-line tools (e.g., `devenv`) allow for automation of common tasks like building, cleaning, and deploying projects.

## Common Command-Line Options

| Option             | Description                                             |
|--------------------|---------------------------------------------------------|
| `/Build`           | Builds the specified solution or project.               |
| `/Rebuild`         | Cleans and then builds the solution or project.         |
| `/Clean`           | Removes all intermediate and output files for settings. |
| `/Deploy`          | Deploys the specified build configuration.              |
| `/Out`             | Redirects output to a file.                             |
| `/Project`         | Specifies the project to build, rebuild, clean, or deploy within a solution. |
| `/ProjectConfig`   | Specifies the project configuration to build.           |

## Usage Examples

### Build a Solution
```bash
devenv MySolution.sln /Build
```

### Rebuild a Project with Debug Configuration
```bash
devenv MySolution.sln /Rebuild Debug /Project MyProject
```

### Clean All Projects in a Solution
```bash
devenv MySolution.sln /Clean
```

### Deploy a Project
```bash
devenv MySolution.sln /Deploy Release /Project MyProject
```

### Redirect Output to a File
```bash
devenv MySolution.sln /Build /Out build_output.txt
```

## Cheat Sheet

- `devenv MySolution.sln /Build`: Build solution.
- `devenv MySolution.sln /Rebuild`: Rebuild solution.
- `devenv MySolution.sln /Clean`: Clean solution.
- `devenv MySolution.sln /Deploy`: Deploy solution.
- `devenv MySolution.sln /Out file.txt`: Redirect output.
