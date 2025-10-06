# Azure CLI (`az`) Command Overview

The `az` command is the primary entry point for interacting with Microsoft Azure via the Azure Command-Line Interface (CLI). It allows users to manage Azure resources and services directly from the terminal.

## Common Options

| Option                        | Description                                               |
|-------------------------------|-----------------------------------------------------------|
| `-h`, `--help`                | Show help information for a command.                      |
| `--version`                   | Display the installed version of Azure CLI.               |
| `-o`, `--output`              | Set output format (e.g., `json`, `table`, `tsv`).         |
| `--subscription`              | Specify the subscription to use.                          |
| `--debug`                     | Show all debug logs for detailed troubleshooting.         |
| `--verbose`                   | Increase verbosity of logs during command execution.      |

## Usage Examples

### Create a Resource Group
```bash
az group create --name MyResourceGroup --location eastus
```

### List Virtual Machines
```bash
az vm list --output table
```

### Start a Virtual Machine
```bash
az vm start --name MyVM --resource-group MyResourceGroup
```

### Create a Storage Account
```bash
az storage account create --name mystorageaccount --resource-group MyResourceGroup --location eastus --sku Standard_LRS
```

### Deploy a Web App
```bash
az webapp up --name MyWebApp --resource-group MyResourceGroup --location eastus
```

## Cheat Sheet

```plaintext
az group create --name <RG_NAME> --location <LOCATION>
az vm list --output table
az vm start --name <VM_NAME> --resource-group <RG_NAME>
az storage account create --name <STORAGE_NAME> --resource-group <RG_NAME> --location <LOCATION> --sku Standard_LRS
az webapp up --name <APP_NAME> --resource-group <RG_NAME> --location <LOCATION>
```
