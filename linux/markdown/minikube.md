## Minikube Command Overview

`minikube` is a tool that allows you to run Kubernetes clusters locally. It is useful for developers who need a local environment for learning Kubernetes, developing with Kubernetes, or testing deployment configurations.

### Common Options

| Option             | Description                                                                         |
|--------------------|-------------------------------------------------------------------------------------|
| `start`            | Starts a local Kubernetes cluster.                                                  |
| `stop`             | Stops the running Kubernetes cluster.                                               |
| `delete`           | Deletes the local Kubernetes cluster.                                               |
| `status`           | Displays the status of the minikube cluster and its components.                     |
| `dashboard`        | Opens the Kubernetes dashboard in the default web browser.                          |
| `config view`      | Displays the current Minikube configuration for easier debugging.                   |
| `addons enable`    | Enables specific Kubernetes addons (e.g., metrics-server).                          |
| `addons disable`   | Disables specific Kubernetes addons.                                                |
| `service`          | Gets the URL for a specific Kubernetes service for easy access from the host.       |
| `logs`             | Shows logs of the Minikube cluster components, useful for troubleshooting.          |

### Usage Examples

1. **Start a Minikube Cluster**

   Start a local cluster with default settings:

   ```bash
   minikube start
   ```

2. **Check Cluster Status**

   View the status of the Minikube cluster components:

   ```bash
   minikube status
   ```

3. **Access Kubernetes Dashboard**

   Launch the Kubernetes dashboard in a web browser:

   ```bash
   minikube dashboard
   ```

4. **Enable Addon**

   Enable the `metrics-server` addon:

   ```bash
   minikube addons enable metrics-server
   ```

5. **Expose Service URL**

   Get the URL for services in the `default` namespace:

   ```bash
   minikube service my-service --url
   ```

6. **View Cluster Logs**

   Display logs for debugging:

   ```bash
   minikube logs
   ```

7. **Stop Minikube**

   Stop the Minikube cluster:

   ```bash
   minikube stop
   ```

8. **Delete Minikube**

   Remove the Minikube cluster:

   ```bash
   minikube delete
   ```

### Cheat Sheet

```plaintext
minikube start                  # Start Minikube cluster
minikube stop                   # Stop Minikube cluster
minikube delete                 # Delete Minikube cluster
minikube status                 # Show cluster status
minikube dashboard              # Open Kubernetes dashboard
minikube addons enable <addon>  # Enable an addon
minikube service <service> --url # Get service URL
minikube logs                   # View cluster logs
```
