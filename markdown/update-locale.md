# `update-locale` Command

The `update-locale` command is used to modify the system's default locale settings on Linux distributions. It updates the `/etc/default/locale` file, which defines the language and regional settings for the system.

## Common Options

| Option        | Explanation                                                |
|---------------|------------------------------------------------------------|
| `LANG=<locale>` | Sets the primary locale for the system.                  |
| `LC_ALL=<locale>` | Overrides all other `LC_*` variables to set a global locale. |
| `LC_MESSAGES=<locale>` | Sets the locale for system messages.               |
| `LC_CTYPE=<locale>` | Sets the locale for character classification and conversion. |
| `LANGUAGE=<language>` | Sets a prioritization list of languages.             |

## Usage Examples

### Set Default Locale to US English
```bash
sudo update-locale LANG=en_US.UTF-8
```

### Set Locale for System Messages to German
```bash
sudo update-locale LC_MESSAGES=de_DE.UTF-8
```

### Clear All Locale Overrides
```bash
sudo update-locale LC_ALL=
```

### Set Multiple Locale Variables
```bash
sudo update-locale LANG=en_US.UTF-8 LC_CTYPE=en_US.UTF-8
```

## Cheat Sheet

```
# Set main locale
sudo update-locale LANG=<locale>

# Override all locale settings
sudo update-locale LC_ALL=<locale>

# Clear specific override
sudo update-locale LC_ALL=

# Set locale for classification
sudo update-locale LC_CTYPE=<locale>
```
