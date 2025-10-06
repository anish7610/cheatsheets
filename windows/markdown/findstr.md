# `findstr` Command in Windows

`findstr` is a command-line utility in Windows used to search for strings within files. It works similarly to `grep` in Linux, allowing you to match patterns or specific text.

## Common Options

| Option     | Description                                                   |
|------------|---------------------------------------------------------------|
| `/B`       | Matches patterns at the beginning of lines.                   |
| `/E`       | Matches patterns at the end of lines.                         |
| `/I`       | Performs a case-insensitive search.                           |
| `/R`       | Interprets search strings as regular expressions.             |
| `/C:"str"` | Searches for an exact string. Useful for strings with spaces. |
| `/N`       | Displays line numbers along with matching lines.              |
| `/S`       | Searches all files in the current directory and subdirectories.|
| `/P`       | Skips files with non-printable characters.                    |

## Usage Examples

### Search for a String in a Specific File
```bash
findstr "error" logfile.txt
```

### Case-Insensitive Search
```bash
findstr /I "warning" logfile.txt
```

### Search for an Exact Phrase
```bash
findstr /C:"critical error" logfile.txt
```

### Search with Regular Expressions
```bash
findstr /R "^ERROR.*failed$" logfile.txt
```

### Include Line Numbers
```bash
findstr /N "failure" logfile.txt
```

### Search Recursively in Directory
```bash
findstr /S "TODO" *.txt
```

## Cheat Sheet

```plaintext
findstr "pattern" file
findstr /I "pattern" file
findstr /C:"exact phrase" file
findstr /R "regex" file
findstr /N "pattern" file
findstr /S "pattern" *.ext
```

Use `findstr` to locate and filter lines containing specific text patterns in files, with options for case sensitivity, exact matches, regular expressions, and recursive directory searching.
