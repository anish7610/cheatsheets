# AWS CloudFormation Command

The `cloudformation` command is part of the AWS CLI, used to create and manage AWS CloudFormation stacks. It allows users to automate the deployment of infrastructure as code on AWS.

## Common Options

| Option                   | Description                                                                             |
|--------------------------|-----------------------------------------------------------------------------------------|
| `create-stack`           | Creates a new CloudFormation stack using a template.                                    |
| `update-stack`           | Updates an existing stack with a new template or parameters.                            |
| `delete-stack`           | Deletes a specified stack.                                                              |
| `describe-stacks`        | Provides details about a stack or stacks.                                               |
| `list-stacks`            | Lists all stacks or stacks with a specific status.                                      |
| `validate-template`      | Validates a CloudFormation template to ensure it is syntactically correct.              |
| `describe-stack-events`  | Retrieves events related to a stack’s changes.                                          |
| `get-template`           | Returns the template used to create or update the stack.                                |

## Usage Examples

### Create a Stack

```bash
aws cloudformation create-stack --stack-name MyStack --template-body file://template.json
```

### Update a Stack

```bash
aws cloudformation update-stack --stack-name MyStack --template-body file://updated-template.json
```

### Delete a Stack

```bash
aws cloudformation delete-stack --stack-name MyStack
```

### Describe Stacks

```bash
aws cloudformation describe-stacks --stack-name MyStack
```

### Validate a Template

```bash
aws cloudformation validate-template --template-body file://template.json
```

## Cheat Sheet

```plaintext
# Create a stack
aws cloudformation create-stack --stack-name <Name> --template-body file://<template-file>

# Update a stack
aws cloudformation update-stack --stack-name <Name> --template-body file://<template-file>

# Delete a stack
aws cloudformation delete-stack --stack-name <Name>

# Describe a stack
aws cloudformation describe-stacks --stack-name <Name>

# Validate a template
aws cloudformation validate-template --template-body file://<template-file>
```
