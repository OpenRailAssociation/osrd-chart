# OSRD Helm Chart Repository

This repository contains Helm charts for deploying OSRD, which consists of three main components:

- **Gateway**: Serves the front end, handles authentication, and proxies requests to the backend.
- **Editoast**: Acts as the backend that interacts with the front end.
- **Core**: Handles computation and business logic.

## Prerequisites

- Kubernetes cluster
- Helm installed


## Deploying the Application

After adding the repository, you can deploy the application using the following command:

```
helm install osrd oci://ghcr.io/osrd-project/charts/osrd --version 0.1.0
```

If you want to use the latest build of the helm chart (not the latest released) you can use

```
helm install osrd oci://ghcr.io/osrd-project/charts/osrd-dev --version 0.1.XXX
```

## Configuration

Check the `values.yaml` file.
