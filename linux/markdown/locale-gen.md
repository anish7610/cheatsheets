# `locale-gen` Command in Linux

`locale-gen` is a command used to generate locale data on a Linux system. Locales define language and regional settings, such as date formats, currency symbols, and character sets.

## Common Options

| Option  | Explanation                                |
|---------|--------------------------------------------|
| `-u`    | Update the locale database without deleting existing locales. |
| `-a`    | Generate all supported locales.            |

## Usage Examples

### Generate Specific Locale
To generate a specific locale like `en_US.UTF-8`:

```bash
sudo locale-gen en_US.UTF-8
```

### Generate All Locales
To generate all locales listed in `/etc/locale.gen`:

```bash
sudo locale-gen
```

### Update Locale Database
To update without removing existing data:

```bash
sudo locale-gen -u
```

## Cheat Sheet

```plaintext
sudo locale-gen <locale>    # Generate specified locale
sudo locale-gen             # Generate enabled locales in /etc/locale.gen
sudo locale-gen -u          # Update locale database
sudo locale-gen -a          # Generate all supported locales
```
