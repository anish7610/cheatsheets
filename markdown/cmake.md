# CMake Command Overview

`cmake` is a cross-platform tool designed to automate the build process of software projects. It uses configuration files called `CMakeLists.txt` to generate build systems for different platforms.

## Common Options

| Option          | Description                                               |
|-----------------|-----------------------------------------------------------|
| `-S <path>`     | Specify the source directory (where CMakeLists.txt is).   |
| `-B <path>`     | Specify the build directory.                              |
| `-D<var>=<val>` | Define a CMake variable.                                  |
| `-G <generator>`| Specify the build system generator.                       |
| `--build <dir>` | Build a project using CMake-generated build system.       |
| `--install <dir>`| Install the compiled build artifacts.                   |
| `--preset <preset>`| Load a preset configuration for build process.         |
| `--version`     | Display CMake version and exit.                           |

## Usage Examples

### Generate a Build System
```bash
cmake -S . -B build/
```

### Build a Project
```bash
cmake --build build/
```

### Set a Build Type
```bash
cmake -S . -B build/ -DCMAKE_BUILD_TYPE=Release
```

### Use a Custom Generator
```bash
cmake -S . -B build/ -G "Ninja"
```

### Install the Project
```bash
cmake --install build/
```

## Cheat Sheet

```bash
# Initialize and configure the project
cmake -S <source_dir> -B <build_dir>

# Build the project
cmake --build <build_dir>

# Set CMake variable
cmake -D<var>=<val>

# Install project
cmake --install <build_dir>
```
