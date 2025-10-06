# Windows Script Host (WSH)

## Description

Windows Script Host (WSH) is a Windows administration tool that provides scripting abilities through compatible languages like VBScript or JScript. It allows the automation of system tasks, configuration management, and interaction with various Windows components.

## Common Options

| Option         | Description                                                       |
|----------------|-------------------------------------------------------------------|
| `/B`           | Batch mode: suppresses user prompts and alerts.                   |
| `/D`           | Displays desktop alerts.                                          |
| `/E:engine`    | Specifies the script engine to use, e.g., VBScript or JScript.    |
| `/H:CScript`   | Sets CScript as the default script host.                          |
| `/H:WScript`   | Sets WScript as the default script host.                          |
| `/I`           | Interactive mode: displays user prompts and alerts.               |
| `/Job:job`     | Executes a job within a .wsf file.                                |
| `/NoLogo`      | Hides the banner displaying the version of the script host being used.|
| `/S`           | Saves current command-line options for use in this session.       |
| `/T:nn`        | Sets the maximum time (in seconds) the script can run.            |
| `/X`           | Executes the script in the debugger.                              |
| `/U`           | Uses Unicode for redirected output from CScript.                  |

## Usage Examples

### Run a VBScript
To run a VBScript file `example.vbs`:

```bash
cscript //NoLogo example.vbs
```

### Run a JScript with a time limit
To run a JScript file `example.js` with a 30-second timeout:

```bash
cscript //T:30 example.js
```

### Set CScript as the default host
To set CScript as the default script host:

```bash
cscript //H:CScript
```

### Execute a job from a .wsf file
To run a specific job named "MyJob" from a `tasks.wsf` file:

```bash
cscript //Job:MyJob tasks.wsf
```

## Cheat Sheet

```plaintext
Run script:                   cscript [options] scriptfile
Suppress logos:               cscript //NoLogo scriptfile
Set default to CScript:       cscript //H:CScript
Set timeout:                  cscript //T:seconds scriptfile
Run with specific engine:     cscript //E:engine scriptfile
Batch mode (no prompts):      cscript //B scriptfile
```

Use these commands to speed up automation tasks and manage script executions effectively.
