# `g++` Command in Linux

`g++` is the GNU C++ compiler, part of the GNU Compiler Collection (GCC). It compiles C++ source files into executable binaries.

## Common Options

| Option       | Explanation                                               |
|--------------|-----------------------------------------------------------|
| `-o <file>`  | Specifies the output file name for the executable.        |
| `-c`         | Compiles source files without linking. Produces `.o` files.|
| `-Wall`      | Enables all standard warnings.                            |
| `-g`         | Generates debug information for use with gdb.             |
| `-O`         | Optimizes the code. Levels: `-O1`, `-O2`, `-O3`.          |
| `-std=<val>` | Specifies the C++ standard (e.g., `-std=c++11`).          |
| `-I<dir>`    | Adds a directory to the list of directories to be searched for header files. |
| `-L<dir>`    | Adds a directory to the list of directories to be searched for libraries.  |
| `-l<name>`   | Links with the specified library.                         |

## Usage Examples

### Compile a Single File

```bash
g++ -o hello hello.cpp
```

### Compile Multiple Files

```bash
g++ -o myprogram main.cpp utils.cpp
```

### Enable All Warnings and Debug Information

```bash
g++ -Wall -g -o debug_program program.cpp
```

### Specify C++ Standard

```bash
g++ -std=c++11 -o modern_cpp_program modern.cpp
```

### Compile and Link with Specific Libraries

```bash
g++ -o app main.cpp -L/usr/local/lib -lsomelibrary
```

### Generate Object Files Only

```bash
g++ -c file1.cpp
g++ -c file2.cpp
g++ -o combined file1.o file2.o
```

## Cheat Sheet

```markdown
# Compilation
g++ -o <output> <source.cpp>
g++ -o <output> <source1.cpp> <source2.cpp>

# Warnings and Debugging
g++ -Wall -g -o <output> <source.cpp>

# C++ Standard
g++ -std=c++17 -o <output> <source.cpp>

# Libraries
g++ -L<dir> -l<lib> -o <output> <source.cpp>

# Optimization Levels
g++ -O2 -o <output> <source.cpp>
```
