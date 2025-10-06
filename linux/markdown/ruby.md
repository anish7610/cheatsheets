# `ruby` Command in Linux

The `ruby` command is used to run Ruby scripts and interact with the Ruby programming language from the command line. Ruby is a dynamic, open-source programming language known for its simplicity and productivity.

## Common Options

| Option      | Description                                              |
|-------------|----------------------------------------------------------|
| `-e 'code'` | Execute the provided Ruby code directly from the command line. |
| `-v`        | Display the Ruby version information.                    |
| `-w`        | Enable warnings. This is useful for debugging.           |
| `-c`        | Check syntax of the script without executing it.         |
| `--verbose` | Enable verbose mode, printing command execution details. |
| `-I dir`    | Add directory to the load path (similar to `require`).   |
| `-r lib`    | Require the specified library before executing the script. |
| `--help`    | Display help information for the `ruby` command.         |

## Usage Examples

### Execute a Ruby Script

```bash
ruby my_script.rb
```

### Check Syntax Only

```bash
ruby -c my_script.rb
```

### Run Inline Ruby Code

```bash
ruby -e 'puts "Hello, World!"'
```

### Run a Script with Warnings and Verbose Output

```bash
ruby -w --verbose my_script.rb
```

### Include Additional Library Paths

```bash
ruby -I lib_dir my_script.rb
```

### Require a Library Before Execution

```bash
ruby -r json -e 'puts JSON.parse("{\"key\": \"value\"}")'
```

## Cheat Sheet

```plaintext
ruby -e 'code'         # Execute Ruby code
ruby -v                # Show Ruby version
ruby -w                # Enable warnings
ruby -c file.rb        # Syntax check only
ruby --verbose file.rb # Verbose mode
ruby -I dir file.rb    # Add directory to load path
ruby -r lib -e 'code'  # Require library before executing code
```

Use this guide to effectively utilize the `ruby` command in your Linux environment.
