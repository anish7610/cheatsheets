# Azure CLI (`az`) Command

The `az` command is a part of the Azure Command-Line Interface (CLI) used to manage Azure resources directly from the command line. It provides a set of commands to automate tasks like deploying and managing virtual machines, web applications, databases, and more.

## Common Options

| Option         | Description                                                    |
|----------------|----------------------------------------------------------------|
| `--version`    | Displays the current version of the Azure CLI.                 |
| `login`        | Authenticates your identity with Azure.                        |
| `account show` | Displays details of the currently logged-in account.           |
| `group list`   | Lists all resource groups within the subscription.             |
| `vm list`      | Lists all virtual machines in the subscription/resource group. |
| `configure`    | Configures defaults, such as region and output format.         |

## Usage Examples

### Login to Azure
```bash
az login
```

### List All Resource Groups
```bash
az group list --output table
```

### Create a Virtual Machine
```bash
az vm create --resource-group MyResourceGroup --name MyVm --image UbuntuLTS --admin-username azureuser --generate-ssh-keys
```

### Show Details of a Specific Virtual Machine
```bash
az vm show --resource-group MyResourceGroup --name MyVm --output json
```

### List All VMs in a Specific Resource Group
```bash
az vm list --resource-group MyResourceGroup --output table
```

## Cheat Sheet

```bash
az login                        # Authenticate with Azure
az account show                 # Show current account
az group list --output table    # List resource groups
az vm create ...                # Create a VM
az vm list --output table       # List VMs
az configure                    # Set defaults
```
