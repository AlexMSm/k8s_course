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

When changing configmaps, create a new one with incremented v1.1 etc. Don't existing as changes won't be applied to pods.

Resources:

Request - What the container requests as a minimum from the k8s nodes
Limit - Actual allowed limits to the container

Essentially a min and max.

Helm

helm create <chart name>
helm install <release-name> <helm chart folder>

minikube tunnel

helm upgrade <release-name> <helm chart folder> --values </values.yaml>

helm ls

For prod/dev, include the namespace in the install/upgrade commands:
helm upgrade <release-name> <helm chart folder> --values </values.yaml> -f <values-dev/prod.yaml> -n <dev/prod>
