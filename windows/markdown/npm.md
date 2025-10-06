# `npm` Command

**Description:**
`npm` (Node Package Manager) is a command-line tool used for installing, managing, and sharing JavaScript packages. It is primarily used in environments running Node.js.

## Common Options

| Option    | Description                                             |
|-----------|---------------------------------------------------------|
| `install` | Install a package or packages.                          |
| `init`    | Create a package.json file interactively.               |
| `update`  | Update all the packages listed in package.json.         |
| `uninstall` | Remove a package.                                    |
| `list`    | List installed packages.                                |
| `outdated`| Check for outdated packages.                            |
| `run`     | Run a script defined in the package.json.               |
| `test`    | Run tests.                                              |
| `start`   | Run the start script defined in the package.json.       |

## Usage Examples

### Install a Package
```bash
npm install express
```

### Initialize a New Project
```bash
npm init
```

### Update All Packages
```bash
npm update
```

### Uninstall a Package
```bash
npm uninstall lodash
```

### List Installed Packages
```bash
npm list
```

### Check for Outdated Packages
```bash
npm outdated
```

### Run a Custom Script
```bash
npm run build
```

### Run Tests
```bash
npm test
```

### Start a Project
```bash
npm start
```

## Cheat Sheet

```plaintext
npm install <package>   # Install a package
npm init                # Initialize a project
npm update              # Update packages
npm uninstall <package> # Uninstall a package
npm list                # List installed packages
npm outdated            # Check outdated packages
npm run <script>        # Run a custom script
npm test                # Run tests
npm start               # Start project
```
