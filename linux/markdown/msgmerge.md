# `msgmerge` Command in Linux

The `msgmerge` command is used to update a translation `.po` file with the latest strings from a `.pot` template. It helps keep translations in sync with source code changes.

## Common Options

| Option       | Explanation                                                                 |
|--------------|-----------------------------------------------------------------------------|
| `-o OUTPUT`  | Specify the output file. By default, updates the input file in place.       |
| `-U`         | Update the input file in place.                                             |
| `--backup`   | Make a backup of the original `.po` file, appending a simple suffix.        |
| `--quiet`    | Suppress verbose output.                                                    |
| `--previous` | Include previous untranslated strings as comments for context.              |
| `--no-fuzzy-matching` | Disable fuzzy matching for strings that no longer match perfectly. |

## Usage Examples

### Update a Translation File

Update a `.po` file with the latest strings from a `.pot` template, modifying the file in place:

```bash
msgmerge -U myfile.po template.pot
```

### Update with Backup

Create a backup of the original `.po` file while updating:

```bash
msgmerge --backup myfile.po template.pot
```

### Update and Specify Output

Update a `.po` file and write to a new output file:

```bash
msgmerge -o updated.po myfile.po template.pot
```

### Suppress Output

Run `msgmerge` without verbose output:

```bash
msgmerge --quiet -U myfile.po template.pot
```

### Include Previous Strings

Retain old translations as comments for reference:

```bash
msgmerge --previous -U myfile.po template.pot
```

## Cheat Sheet

```plaintext
msgmerge -U file.po template.pot        # Update .po file in place
msgmerge -o out.po file.po template.pot # Output to new file
msgmerge --backup file.po template.pot  # Backup original file
msgmerge --quiet -U file.po template.pot # Suppress output
```
