# `tzselect` Command

`tzselect` is an interactive command-line tool used to set the time zone for your system. It helps users identify the correct timezone without changing the system configuration files.

## Common Options

| Option | Explanation                                           |
|--------|-------------------------------------------------------|
| None   | `tzselect` does not use command-line options. It is purely interactive. |

## Usage Examples

### Example 1: Setting Timezone
Simply type `tzselect` in the terminal and follow the interactive prompts to select your region, country, and timezone.

```bash
tzselect
```

### Example 2: Redirect Output
Capture the result of `tzselect` and apply it elsewhere using environment variables.

```bash
TZ=$(tzselect)
echo "Timezone set to $TZ"
```

## Cheat Sheet

```plaintext
# Run tzselect
tzselect

# Set timezone to variable
TZ=$(tzselect)
```

This process doesn't modify system files directly. It informs you of the correct timezone string to use, often for personal shell environments.
