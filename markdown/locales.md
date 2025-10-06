# `locales` Command in Linux

The `locales` command in Linux is used to display information related to locale settings that define the language, region, and character encoding used by applications.

## Common Options

| Option            | Description                                      |
|-------------------|--------------------------------------------------|
| `-a`              | Displays all available locales on the system.    |
| `-c`              | Outputs details of the current locale settings.  |
| `-v`              | Verbose output showing more locale information.  |

## Usage Examples

### List All Available Locales
To see all the locales installed on your system:

```bash
locale -a
```

### View Current Locale Settings
To display the current settings of your locale environment variables:

```bash
locale
```

### Detailed Locales Information
To get detailed information about your current settings:

```bash
locale -c
```

### Verbose Output
For verbose output:

```bash
locale -v
```

## Cheat Sheet

```plaintext
# List all available locales
locale -a

# Show current locale settings
locale

# Show details of current locale settings
locale -c

# Verbose output of locale info
locale -v
```

This guide provides a concise overview for quickly understanding and using the `locales` command.
