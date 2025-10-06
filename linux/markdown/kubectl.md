# `kubectl` Command

`kubectl` is the command-line tool for interacting with Kubernetes clusters. It allows administrators and developers to deploy, manage, monitor, and troubleshoot applications within the Kubernetes environment.

## Common Options

| Option                   | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| `get`                    | List resources (e.g., pods, services, deployments).                         |
| `describe`               | Show detailed information about a specific resource.                        |
| `create`                 | Create a resource from a file or stdin.                                     |
| `apply`                  | Apply a configuration to a resource by filename or stdin.                   |
| `delete`                 | Delete resources by file, stdin, resource name, or label selector.          |
| `logs`                   | Print the logs for a container in a pod.                                    |
| `exec`                   | Execute a command in a container.                                           |
| `config`                 | Modify `kubectl` configuration files.                                       |
| `scale`                  | Scale a deployment, replica set, or replication controller.                 |
| `edit`                   | Edit a resource on the server.                                              |
| `port-forward`           | Forward one or more local ports to a pod.                                   |
| `get nodes`              | List all nodes in the cluster.                                              |
| `version`                | Display the `kubectl` and server version information.                       |

## Usage Examples

### List All Pods
```bash
kubectl get pods
```

### Show Detailed Information About a Pod
```bash
kubectl describe pod my-pod
```

### Create a Resource from a YAML File
```bash
kubectl create -f my-resource.yaml
```

### Apply Changes from a YAML File
```bash
kubectl apply -f my-changes.yaml
```

### Delete a Deployment
```bash
kubectl delete deployment my-deployment
```

### View Logs from a Specific Pod
```bash
kubectl logs my-pod
```

### Execute a Command in a Running Container
```bash
kubectl exec -it my-pod -- /bin/bash
```

### Scale a Deployment to 3 Replicas
```bash
kubectl scale deployment my-deployment --replicas=3
```

### Edit an Existing Resource
```bash
kubectl edit deployment my-deployment
```

### Forward Local Port 8080 to Port 80 on a Pod
```bash
kubectl port-forward my-pod 8080:80
```

## Cheat Sheet

```plaintext
kubectl get pods
kubectl describe pod <pod-name>
kubectl create -f <file.yaml>
kubectl apply -f <file.yaml>
kubectl delete <resource> <resource-name>
kubectl logs <pod-name>
kubectl exec -it <pod-name> -- <command>
kubectl scale deployment <name> --replicas=<num>
kubectl edit <resource> <resource-name>
kubectl port-forward <pod-name> <local-port>:<pod-port>
```
