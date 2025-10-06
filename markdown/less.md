# `less` Command in Linux

## Description
The `less` command is a pager utility in Linux that allows you to view and navigate through the contents of text files one screen at a time. Unlike `more`, `less` supports both forward and backward scrolling.

## Common Options

| Option | Description                                      |
|--------|--------------------------------------------------|
| `-N`   | Show line numbers.                               |
| `-S`   | Disable line wrapping (long lines are not folded).|
| `-X`   | Disable clearing the screen when exiting.        |
| `-g`   | Highlight the last search result.                |
| `-i`   | Ignore case in searches.                         |

## Usage Examples

### Viewing a File with Line Numbers
```bash
less -N filename.txt
```

### Viewing a File Without Line Wrapping
```bash
less -S filename.txt
```

### Searching Text (Case Insensitive)
```bash
less -i filename.txt
# Then type `/searchtext` and press `Enter`.
```

### Exiting Without Clearing the Screen
```bash
less -X filename.txt
```

## Cheat Sheet

```plaintext
Space   : Next page
b       : Previous page
/term   : Search forward for 'term'
?term   : Search backward for 'term'
n       : Next search result
N       : Previous search result
q       : Quit
h       : Help
```

This compact reference provides a quick overview for using `less` effectively in everyday tasks.
