# `gcc` Command Overview

`gcc` is the GNU Compiler Collection, used to compile C and C++ programs. It transforms source code into executable binaries.

## Common Options

| Option        | Description                                          |
|---------------|------------------------------------------------------|
| `-o <file>`   | Specify the output file name                         |
| `-c`          | Compile source files without linking                 |
| `-g`          | Generate debug information for use with gdb          |
| `-Wall`       | Enable all standard warnings                         |
| `-Werror`     | Treat warnings as errors                             |
| `-O`          | Enable basic optimization                            |
| `-O2`         | Enable a good level of optimization                  |
| `-std=<type>` | Specify the standard (e.g., `-std=c99`, `-std=c++11`)|

## Usage Examples

### Compile a C Program

Compile `program.c` and output to `program`:

```bash
gcc -o program program.c
```

### Compile with Debug Information

Compile with debugging symbols for gdb:

```bash
gcc -g -o program program.c
```

### Compile Without Linking

Compile to object file `program.o`:

```bash
gcc -c program.c
```

### Compile with Warnings Enabled

Compile and show standard warnings:

```bash
gcc -Wall -o program program.c
```

### Optimize and Compile

Compile with optimizations:

```bash
gcc -O2 -o program program.c
```

## Cheat Sheet

```plaintext
Compile:           gcc -o output source.c
Compile with debug: gcc -g -o output source.c
Warnings:          gcc -Wall -o output source.c
Optimize:          gcc -O2 -o output source.c
```
