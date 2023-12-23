Files are considered ephemeral - files are lost when a container or pod is replaced.
K8s volumes persist data.

ConfigMaps

- key-value pairs for plain text data
- Used to inject config into pod containers

Secrets

- k-v pairs for secret data
- Used for passwords and api keys

Namespace
Where all k8s resources are created - set to 'default' by default.
