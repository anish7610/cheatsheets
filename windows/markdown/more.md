# `more` Command in Windows

The `more` command in Windows is used to view the contents of a text file one screen at a time, making it easier to handle large file outputs.

## Common Options

| Option         | Explanation                                             |
|----------------|---------------------------------------------------------|
| `/E`           | Enables extended features that allow additional commands within `more`. |
| `/C`           | Clears the screen before displaying content.            |

## Usage Examples

### Viewing a File

Display `example.txt` with content shown one screen at a time:

```bash
type example.txt | more
```

### Clearing Screen Before Display

Clear the screen before displaying the contents of `example.txt`:

```bash
type example.txt | more /C
```

### Using Extended Features

Use the `/E` option to enable commands like navigating backwards:

```bash
type example.txt | more /E
```

## Cheat Sheet

```plaintext
type filename.txt | more       # View file page by page
type filename.txt | more /C    # Clear screen before display
type filename.txt | more /E    # Enable extended features
```
