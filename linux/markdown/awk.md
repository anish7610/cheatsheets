# awk Command in Linux

`awk` is a powerful text processing tool used for pattern scanning and processing. It interprets a special-purpose programming language to search, process, and generate reports based on text data.

## Common Options

| Option  | Explanation                                           |
|---------|-------------------------------------------------------|
| -F      | Defines the input field separator.                    |
| -v      | Assigns a variable.                                   |
| -f      | Reads the awk program from a file.                    |

## Usage Examples

### Example 1: Print Specific Columns

```bash
awk '{print $1, $3}' file.txt
```
*Prints the 1st and 3rd columns of each line from `file.txt`.*

### Example 2: Use Custom Field Separator

```bash
awk -F: '{print $1, $3}' /etc/passwd
```
*Prints the username and UID from the `/etc/passwd` file, using `:` as a field separator.*

### Example 3: Conditional Printing

```bash
awk '$3 > 100 {print $1, $3}' file.txt
```
*Prints the 1st and 3rd columns only if the 3rd column is greater than 100.*

### Example 4: Calculate Sum

```bash
awk '{sum += $2} END {print sum}' file.txt
```
*Calculates the sum of values in the 2nd column.*

## Cheat Sheet

```plaintext
awk '{print $1}' file.txt                  # Print first column
awk -F: '{print $1}' file.txt              # Use ':' as field separator
awk '$3 > 100 {print $0}' file.txt         # Print lines where 3rd column > 100
awk '{sum += $2} END {print sum}' file.txt # Calculate sum of 2nd column
awk -v var=5 '$1 < var {print $1}' file.txt # Use variable for condition
```

Use these concise examples and shortcuts to efficiently handle text processing tasks with `awk`.
