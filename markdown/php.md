# PHP Command in Linux

The `php` command is used to run PHP scripts on the command line. It can execute `.php` files and evaluate PHP code directly from the terminal.

## Common Options

| Option        | Description                                                                 |
|---------------|-----------------------------------------------------------------------------|
| `-a`          | Run PHP interactively (interactive shell).                                  |
| `-f <file>`   | Parse and execute the specified file.                                       |
| `-r <code>`   | Run PHP code without using a script file.                                   |
| `-l`          | Syntax check only (lint).                                                   |
| `-i`          | Show PHP configuration information (same as `phpinfo()` function).          |
| `-v`          | Display the PHP version.                                                    |
| `-m`          | List compiled-in modules.                                                   |
| `-S <addr:port>` | Start a built-in web server at given address and port (e.g., `localhost:8000`). |

## Usage Examples

### Running a PHP File
```bash
php -f script.php
```

### Running PHP Code
```bash
php -r 'echo "Hello, World!\n";'
```

### Checking Syntax
```bash
php -l script.php
```

### Using Interactive Mode
```bash
php -a
```

### Displaying PHP Version
```bash
php -v
```

### Starting a Local Development Server
```bash
php -S localhost:8000
```

## Cheat Sheet

```plaintext
php -f <file>       # Execute PHP file
php -r <code>       # Run PHP code from command line
php -l <file>       # Syntax check
php -a              # Interactive mode
php -v              # PHP version
php -S localhost:8000 # Start built-in server
```

Use this guide to quickly reference the `php` command and its most useful options for running and testing PHP scripts efficiently.
