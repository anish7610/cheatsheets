# Perl Command in Linux

The `perl` command runs the Perl programming language interpreter. Perl is a versatile scripting language often used for text processing, system administration, and web development.

## Common Options

| Option        | Description                                              |
|---------------|----------------------------------------------------------|
| `-e`          | Execute a Perl script provided on the command line.      |
| `-p`          | Loop over input line-by-line, print each line after processing.|
| `-i`          | Edit files in place (use with caution).                  |
| `-n`          | Loop over input line-by-line without auto-printing.      |
| `-l`          | Enable automatic line-ending processing.                 |
| `-M`          | Use a specific Perl module.                              |
| `-a`          | Enable autosplit mode for `-n` or `-p` (often used with `-F`).|
| `-F`          | Specify input field separator when using `-a`.           |
| `-c`          | Check syntax only, don’t execute.                        |

## Usage Examples

### Simple Text Processing

Capitalize the first letter of each word in a text file:

```bash
perl -pe 's/\b(\w)/\U$1/g' file.txt
```

### In-place Editing

Replace all occurrences of 'foo' with 'bar' in a file:

```bash
perl -pi -e 's/foo/bar/g' file.txt
```

### Reading from Standard Input

Print every line containing 'error':

```bash
perl -ne 'print if /error/' log.txt
```

### Splitting Fields with Autosplit

Print the second column from a colon-separated file:

```bash
perl -F: -lane 'print $F[1]' data.txt
```

## Cheat Sheet

```plaintext
perl -e 'code'          # Execute one-liner
perl -pe 's/foo/bar/g'  # Substitute text
perl -pi -e '...' file  # In-file edit
perl -ne 'print if /.../'  # Conditional print
perl -F: -lane '...'    # Split fields and execute
```

Use these commands to leverage Perl's powerful text manipulation capabilities efficiently in your Linux environment.
