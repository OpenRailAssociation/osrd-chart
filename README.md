# OSRD Helm Chart Repository

# ARCHIVED REPOSITORY

Find the current chart in the main osrd repo here: https://github.com/OpenRailAssociation/osrd/tree/dev/chart

---------

This repository contains Helm charts for deploying OSRD, which consists of three main components:

- **Gateway**: Serves the front end, handles authentication, and proxies requests to the backend.
- **Editoast**: Acts as the backend that interacts with the front end.
- **Core**: Handles computation and business logic.

## Prerequisites

- Kubernetes cluster
- Helm installed

## Deploying the application

After adding the repository, you can deploy the application using the following command:

```
helm install osrd oci://ghcr.io/openrailassociation/osrd-charts/osrd --version 0.1.0
```

If you want to use the latest build of the helm chart (not the latest released) you can use

```
helm install osrd oci://ghcr.io/openrailassociation/osrd-charts/osrd-dev --version 0.1.XXX
```

## Configuration

Check the `values.yaml` file.


## Contributing

To comply with the [DCO](http://developercertificate.org/), all commits must
include a Signed-off-by line. You can find more information about this [here](https://osrd.fr/en/docs/guides/contribute/contribute-code/commit-conventions/#the-developer-certificate-of-origin)

For more advice on how to contribute, follow that link:
https://osrd.fr/en/docs/guides/contribute/contribute-code
