# `gettext` Command in Linux

`gettext` is a command-line utility used for internationalization and localization, primarily by providing translated text for applications. It retrieves translated strings from compiled message catalogs (usually `.mo` files).

## Common Options

| Option       | Description                                           |
|--------------|-------------------------------------------------------|
| `-d`         | Specify the text domain (i.e., the base name of the MO file). |
| `-e`         | Enable extended quoting.                              |
| `--help`     | Display a help message with usage information.        |
| `--version`  | Output version information of `gettext`.              |

## Usage Examples

### 1. Retrieve a Translated String

Print a translated string from the specified domain:

```bash
gettext -d mydomain "Hello, World"
```

### 2. Using Extended Quoting

Enable extended quoting for special characters:

```bash
gettext -e -d mydomain "He said, \"Hello, World!\""
```

### 3. Check Available Version

Check the installed version of `gettext`:

```bash
gettext --version
```

## Cheat Sheet

```plaintext
# Basic syntax
gettext [-d DOMAIN] [TEXT]

# Retrieve translation
gettext -d domain "Text"

# Extended quoting
gettext -e -d domain "Text with \"quotes\""
```
