# `gcloud` Command Overview

The `gcloud` command is part of the Google Cloud SDK and is used to interact with Google Cloud Platform (GCP) services. It allows users to manage resources and applications hosted on GCP.

## Common Options

| Option                          | Description                                               |
|---------------------------------|-----------------------------------------------------------|
| `init`                          | Initialize or reinitialize gcloud.                        |
| `help`                          | Display help for gcloud commands.                         |
| `config set`                    | Set a specific configuration value.                       |
| `config list`                   | List the active configuration values.                     |
| `auth login`                    | Authorize gcloud to access GCP resources.                 |
| `projects list`                 | List all projects you have access to.                     |
| `compute instances list`        | List compute engine instances.                            |
| `compute ssh`                   | SSH into a compute engine instance.                       |
| `app deploy`                    | Deploy an application to App Engine.                      |
| `beta`                          | Access beta features and commands.                        |

## Usage Examples

### Initializing the SDK

```sh
gcloud init
```

### Listing Projects

```sh
gcloud projects list
```

### Setting a Configuration Value

```sh
gcloud config set project [PROJECT_ID]
```

### SSH into a Compute Engine Instance

```sh
gcloud compute ssh [INSTANCE_NAME] --zone [ZONE]
```

### Deploying an App to App Engine

```sh
gcloud app deploy
```

## Cheat Sheet

- **Initialize**: `gcloud init`
- **Login**: `gcloud auth login`
- **Set Project**: `gcloud config set project [PROJECT_ID]`
- **List Projects**: `gcloud projects list`
- **List Instances**: `gcloud compute instances list`
- **SSH Instance**: `gcloud compute ssh [INSTANCE_NAME] --zone [ZONE]`
- **Deploy App**: `gcloud app deploy`

Use these commands to efficiently manage GCP resources from the command line.
