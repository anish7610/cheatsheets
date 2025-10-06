# `npm` Command in Linux

`npm` stands for Node Package Manager. It is a command-line tool used to manage Node.js packages. With `npm`, users can install, update, and manage Node.js software packages.

## Common Options

| Option                      | Description                                                   |
|-----------------------------|---------------------------------------------------------------|
| `-v`, `--version`           | Display the npm version.                                      |
| `install <package>`         | Install a specified package and added it to `package.json`.   |
| `uninstall <package>`       | Remove a specified package.                                   |
| `update <package>`          | Update a specified package to the latest version.             |
| `list`, `ls`                | List installed packages.                                      |
| `init`                      | Create a new `package.json` file interactively.               |
| `start`                     | Run the start script defined in `package.json`.               |
| `test`                      | Run the test script defined in `package.json`.                |
| `run <script>`              | Run a script specified in `package.json`.                     |

## Usage Examples

### Install a Package

```bash
npm install express
```

### Uninstall a Package

```bash
npm uninstall express
```

### Update a Package

```bash
npm update express
```

### List Installed Packages

```bash
npm list
```

### Initialize a Project

```bash
npm init
```

### Run a Start Script

```bash
npm start
```

### Run a Test Script

```bash
npm test
```

## Cheat Sheet

```plaintext
npm -v                         # Show npm version
npm install <package>          # Install a package
npm uninstall <package>        # Remove a package
npm update <package>           # Update a package
npm list                       # List installed packages
npm init                       # Initialize a new project
npm start                      # Run the start script
npm test                       # Run the test script
```
