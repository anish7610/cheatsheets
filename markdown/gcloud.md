# `gcloud` Command Overview

The `gcloud` command is a part of the Google Cloud SDK and is used to manage Google Cloud resources and developer workflow through the command line.

## Common Options

| Option               | Explanation                                          |
|----------------------|------------------------------------------------------|
| `--project`          | Specifies the Google Cloud project to use.           |
| `--zone`             | Specifies the zone for zonal resources.              |
| `--region`           | Specifies the region for regional resources.         |
| `--quiet` or `-q`    | Disables all interactive prompts.                    |
| `--format`           | Specifies the output format (e.g., `json`, `yaml`).  |
| `--help`             | Displays help information about the command.         |

## Usage Examples

### List All Projects

```bash
gcloud projects list
```

### Create a New VM Instance

```bash
gcloud compute instances create my-instance --zone=us-central1-a
```

### Deploy an App to App Engine

```bash
gcloud app deploy
```

### Set the Default Project

```bash
gcloud config set project my-project-id
```

### Get Credentials for a GKE Cluster

```bash
gcloud container clusters get-credentials my-cluster --zone=us-central1-a
```

## Cheat Sheet

```plaintext
# List projects
gcloud projects list

# Create VM instance
gcloud compute instances create my-instance --zone=ZONE

# Deploy to App Engine
gcloud app deploy

# Set default project
gcloud config set project PROJECT_ID

# Get GKE cluster credentials
gcloud container clusters get-credentials CLUSTER_NAME --zone=ZONE
```
