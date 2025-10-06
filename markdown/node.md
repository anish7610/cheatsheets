## `node` Command

`node` is the command-line interface for running JavaScript code outside the browser, using the Node.js runtime. It is widely used for developing and running server-side applications.

### Common Options

| Option         | Description                                              |
|----------------|----------------------------------------------------------|
| `-v`, `--version` | Print the Node.js version.                               |
| `-e`           | Execute JavaScript code passed as a string.              |
| `-p`           | Print the result of the code to the standard output.     |
| `--check`      | Syntax check the script without executing.               |
| `--inspect`    | Activate the V8 inspector for debugging.                 |
| `--require` or `-r` | Load modules before running the script.                 |

### Usage Examples

- **Run a JavaScript file:**
  ```bash
  node app.js
  ```

- **Print Node.js version:**
  ```bash
  node -v
  ```

- **Execute JavaScript code directly:**
  ```bash
  node -e "console.log('Hello, World!')"
  ```

- **Syntax check a file:**
  ```bash
  node --check app.js
  ```

- **Debug with V8 inspector:**
  ```bash
  node --inspect app.js
  ```

- **Require a module before running a script:**
  ```bash
  node -r dotenv/config app.js
  ```

### Cheat Sheet

```plaintext
Run file: node <file>
Version: node -v
Execute: node -e "<code>"
Syntax check: node --check <file>
Debug: node --inspect <file>
Require module: node -r <module> <file>
```
