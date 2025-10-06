# `locale` Command in Linux

The `locale` command is used to display or set the current language and regional settings, such as date formats, currency symbols, and character encoding. These settings influence how programs handle and display these data types.

## Common Options

| Option      | Description                                                   |
|-------------|---------------------------------------------------------------|
| `-a`        | Show all available locale definitions.                        |
| `-m`        | Display all available character maps.                         |
| `-k`        | Display key names and values for the current locale settings. |
| `-c`        | Print information in a more human-readable format.            |

## Usage Examples

### Display All Available Locales

```bash
locale -a
```

### Show Current Locale Settings

```bash
locale
```

### Check Only Specific Locale Category (e.g., Time)

```bash
locale time
```

### Display Locale Definitions with Key Names and Values

```bash
locale -k
```

## Cheat Sheet

```plaintext
# List all available locales
locale -a

# Show current locale settings
locale

# Check specific locale category
locale [category_name]

# Display all character maps
locale -m

# Display settings with key names
locale -k
```
