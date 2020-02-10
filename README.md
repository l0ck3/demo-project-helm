# Garden Demo with Helm

This is an example project for reproducing the following issue: https://github.com/garden-io/garden/issues/1583

## Versions

- Docker Desktop (Mac) 2.2.0.0
- Garden 0.11.2
- Helm 3.0.3

## How to reproduce

Launch Garden in Dev mode

```
$ garden dev
```

Open the UI in the browser

Access the `Logs` tab


## Problem

When opening the UI, the Helm modules folder will be deleted from the `.garden/build` directory.

Garden will log the following errors in the terminal:

```
[...]
Error: open /.../demo-project-helm/.garden/build/backend/garden-values.yml: no such file or directory
[...]
```
