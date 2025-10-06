# Linux `grep` Command

The `grep` command searches for patterns within files or input text and prints lines that match the specified pattern. It is often used for filtering text and locating specific data in files.

## Common Options

| Option       | Description                                        |
|--------------|----------------------------------------------------|
| `-i`         | Ignore case distinctions in patterns and data.     |
| `-v`         | Invert match; select non-matching lines.           |
| `-r` or `-R` | Recursively search directories.                    |
| `-c`         | Count the number of matching lines.                |
| `-n`         | Prefix each line of output with the line number.   |
| `-l`         | List only filenames with matching lines.           |
| `-w`         | Match whole words only.                            |
| `-e`         | Specify multiple patterns.                         |

## Usage Examples

### Search for a String in a File
```bash
grep "search_term" filename.txt
```

### Case-Insensitive Search
```bash
grep -i "search_term" filename.txt
```

### Search Recursively in a Directory
```bash
grep -r "search_term" /path/to/directory
```

### Count Occurrences of a Pattern
```bash
grep -c "search_term" filename.txt
```

### Display Line Numbers with Matches
```bash
grep -n "search_term" filename.txt
```

### Invert Match (Show Non-Matching Lines)
```bash
grep -v "string_to_exclude" filename.txt
```

### Search for Multiple Patterns
```bash
grep -e "pattern1" -e "pattern2" filename.txt
```

## Cheat Sheet

```
# Basic use:
grep "pattern" file      # Find pattern in file
grep -i "pattern" file   # Case-insensitive search

# Details:
grep -n "pattern" file   # Show line numbers
grep -c "pattern" file   # Count matches
grep -v "pattern" file   # Show lines without match

# Advanced:
grep -r "pattern" dir    # Recursive search in directory
grep -w "word" file      # Match whole words only
```
