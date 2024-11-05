# helm-rtsp-to-web

This repo contains base file to deploy rtsp-to-web under Kubernetes using Helm

## Customize

- **config.json**: set the rtsp cameras definitions.
- **values.yaml**: kubernetes deployment values.

## Usage

### Test

``` bash
helm install --dry-run --debug rtsp-to-web .
```

### Create deployment files

``` bash
helm template --debug rtsp-to-web .
```

### Install

```bash
helm install --create-namespace --namespace rtsp-to-web rtsp-to-web .
```
### Upgrade

```bash
helm upgrade rtsp-to-web .
```

### Delete

```bash
helm delete rtsp-to-web
```