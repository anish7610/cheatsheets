# `more` Command Overview

The `more` command in Linux is a simple pager used to view the contents of a text file one screen at a time. It's useful for reading through long files.

## Common Options

| Option | Description                          |
|--------|--------------------------------------|
| `-d`   | Displays a prompt and error message. |
| `-c`   | Clears the screen before displaying. |
| `-f`   | Counts logical lines instead of screen lines. |
| `-p`   | Scrolls by clearing the screen.      |
| `-s`   | Squeezes multiple blank lines into one. |
| `-n`   | Specifies the number of lines per page. |

## Usage Examples

### Basic File Viewing

```bash
more example.txt
```
View `example.txt` one screen at a time.

### View with Squeezed Blank Lines

```bash
more -s example.txt
```
Collapse multiple blank lines into one.

### Clear Screen Between Pages

```bash
more -c largefile.log
```
Clear the screen before displaying each page of `largefile.log`.

### Define Number of Lines Per Page

```bash
more -5 example.txt
```
Display 5 lines at a time from `example.txt`.

## Cheat Sheet

```plaintext
more filename           # View file one screen at a time
more -s filename        # Squeeze blank lines
more -c filename        # Clear screen before each page
more -nX filename       # Display X lines per page
q                       # Quit viewing
```
