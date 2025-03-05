# Kannika Armory and Kustomize example

This repository contains example configurations for deploying Kannika Armory using Kustomize.

### Prerequisites

- [Kustomize](https://kustomize.io/)
- [Helm](https://helm.sh/)
- [kubectl](https://kubernetes.io/docs/reference/kubectl/overview/)

### Usage

```sh
# Use the default chart
kustomize build --enable-helm base/ 
```

```sh
# Use the default chart with Roles instead of ClusterRoles
kustomize build --enable-helm overlays/replace-rbac/
```