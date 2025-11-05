---
title: Kubernetes
type: docs
sidebar:
  open: true
---

## Common Commands

### kubectl autocomplete

**Bash**

```bash
source <(kubectl completion bash) # set up autocomplete in bash into the current shell, bash-completion package should be installed first.
echo "source <(kubectl completion bash)" >> ~/.bashrc # add autocomplete permanently to your bash shell.
```

### Shell into pod

```bash
kubectl exec -it <pod> -n <namespace> -- sh
```

### Set the default namespace for the current context

```bash
kubectl config set-context --current --namespace=<your-namespace>
```

### Others

- https://kubernetes.io/docs/reference/kubectl/quick-reference/
