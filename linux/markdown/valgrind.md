# Valgrind Command Overview

Valgrind is a programming tool used for memory debugging, memory leak detection, and profiling. It helps developers identify issues such as invalid memory use, illegal memory access, and memory leaks.

## Common Options

| Option                | Description                                                                     |
|-----------------------|---------------------------------------------------------------------------------|
| `--leak-check=<yes|no>` | Enables or disables detailed memory leak checking. Default is `no`.             |
| `--track-origins=<yes|no>` | Tracks the origin of uninitialized values. Default is `no`.                    |
| `--show-reachable=<yes|no>` | Displays details of still-reachable blocks at exit. Default is `no`.          |
| `--log-file=<filename>` | Writes Valgrind output to the specified file instead of standard error.        |
| `--tool=<toolname>`   | Specifies which Valgrind tool to use (e.g., `memcheck`, `cachegrind`).           |

## Usage Examples

### Checking for Memory Leaks

```bash
valgrind --leak-check=yes ./my_program
```

### Output Results to a File

```bash
valgrind --log-file=valgrind_output.txt ./my_program
```

### Track the Origin of Uninitialized Values

```bash
valgrind --track-origins=yes ./my_program
```

### Use a Specific Valgrind Tool

```bash
valgrind --tool=cachegrind ./my_program
```

## Quick Reference Cheat Sheet

```plaintext
valgrind --leak-check=yes ./program       # Check memory leaks
valgrind --log-file=output.txt ./program  # Redirect output to file
valgrind --track-origins=yes ./program    # Track uninitialized memory
valgrind --tool=toolname ./program        # Use specified tool
```
