# `iconv` Command Overview

`iconv` is a command-line utility used to convert text from one character encoding to another. It's commonly used for ensuring proper text encoding compatibility between different systems or applications.

## Common Options

| Option         | Description                                                  |
|----------------|--------------------------------------------------------------|
| `-f FROMENC`   | Specifies the source character encoding.                     |
| `-t TOENC`     | Specifies the target character encoding.                     |
| `-o FILE`      | Writes output to a specific file (default is standard output).|
| `-l`           | Lists all known character encodings.                         |

## Usage Examples

### Convert a File's Encoding

Convert a file from ISO-8859-1 to UTF-8 encoding:

```bash
iconv -f ISO-8859-1 -t UTF-8 input.txt -o output.txt
```

### Convert Standard Input

Convert text from standard input from UTF-16 to UTF-8:

```bash
echo "Hello, 世界" | iconv -f UTF-16 -t UTF-8
```

### Display Available Encodings

List all available character encodings:

```bash
iconv -l
```

## Cheat Sheet

```bash
# Convert file encoding
iconv -f FROMENC -t TOENC input.txt -o output.txt

# Convert standard input
echo "text" | iconv -f FROMENC -t TOENC

# List available encodings
iconv -l
```
