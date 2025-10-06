# pip Command in Linux

`pip` is a package manager for Python that allows you to install, upgrade, and manage Python packages from the Python Package Index (PyPI).

## Common Options

| Option                | Description                                    |
|-----------------------|------------------------------------------------|
| `install <package>`   | Install a package                              |
| `uninstall <package>` | Uninstall a package                            |
| `list`                | List installed packages                        |
| `show <package>`      | Display information about a package            |
| `freeze`              | Output installed packages in requirements format |
| `--upgrade`           | Upgrade a package to the latest version        |
| `--user`              | Install/upgrade packages per user              |

## Usage Examples

1. **Install a Package**

   ```bash
   pip install requests
   ```

2. **Uninstall a Package**

   ```bash
   pip uninstall requests
   ```

3. **List All Installed Packages**

   ```bash
   pip list
   ```

4. **Show Package Information**

   ```bash
   pip show requests
   ```

5. **Freeze Installed Packages to a File**

   ```bash
   pip freeze > requirements.txt
   ```

6. **Upgrade a Package**

   ```bash
   pip install --upgrade requests
   ```

7. **Install a Package for the Current User Only**

   ```bash
   pip install --user numpy
   ```

## Cheat Sheet

```plaintext
Install:       pip install <package>
Uninstall:     pip uninstall <package>
List:          pip list
Show:          pip show <package>
Freeze:        pip freeze > requirements.txt
Upgrade:       pip install --upgrade <package>
User Install:  pip install --user <package>
```
