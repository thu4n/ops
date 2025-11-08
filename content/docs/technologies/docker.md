---
title: Docker
type: docs
sidebar:
  open: true
---

## Common Commands

### Remove all unused images

```bash
 docker image prune
```

Remove all dangling images. If `-a` is specified, also remove all images not referenced by any container.

### Buid and push multi-arch image

```bash
docker buildx build --platform=linux/amd64,linux/arm64 --push --tag your-username/multiarch-example:buildx-latest .
```

### Others

- https://docs.docker.com/get-started/docker_cheatsheet.pdf
