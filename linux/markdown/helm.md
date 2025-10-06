### Helm Command Overview

`helm` is a package manager for Kubernetes that helps you find, share, and use software built for Kubernetes. It manages Kubernetes applications through Helm Charts, which are packages of pre-configured Kubernetes resources.

### Common Options

| Option           | Description                                               |
|------------------|-----------------------------------------------------------|
| `install`        | Install a Helm chart.                                     |
| `upgrade`        | Upgrade a release to a new chart or version.              |
| `uninstall`      | Uninstall a Helm chart.                                   |
| `list`           | List all Helm releases.                                   |
| `repo add`       | Add a chart repository.                                   |
| `repo update`    | Update information of available charts.                   |
| `search hub`     | Search for charts in the Helm Hub.                        |
| `search repo`    | Search for charts in the local repositories.              |
| `dependency`     | Manage chart dependencies.                                |
| `status`         | Display the status of a named release.                    |
| `template`       | Generate Kubernetes manifest files from a chart.          |

### Usage Examples

#### Install a Chart
```bash
helm install my-release stable/mysql
```

#### Upgrade a Release
```bash
helm upgrade my-release stable/mysql --version 1.5.0
```

#### Uninstall a Chart
```bash
helm uninstall my-release
```

#### List all Releases
```bash
helm list
```

#### Add a Repository
```bash
helm repo add stable https://charts.helm.sh/stable
```

#### Update Chart Repositories
```bash
helm repo update
```

#### Search for a Chart in Repositories
```bash
helm search repo mysql
```

### Quick Reference Cheat Sheet

```plaintext
helm install <release-name> <chart>
helm upgrade <release-name> <chart> --version <version>
helm uninstall <release-name>
helm list
helm repo add <name> <url>
helm repo update
helm search repo <keyword>
```
