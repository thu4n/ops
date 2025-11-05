---
title: Container OOMKilled
type: docs
sidebar:
  open: true
---

**`OOMKilled`** (Out of Memory Killed) is a kernel-level event where the system terminates a process for exceeding its allocated memory limit. In Kubernetes, this results in a pod restart with `Exit Code 137`.

## Symptoms

- Pod status shows `OOMKilled`.
- Container restarts frequently.
- Application crashes with exit code 137.
- Kubernetes events show memory limit exceeded.

## Solutions

- For a quick fixing attempt, try increasing the memory request and limit for the container.

## References

1. https://lumigo.io/kubernetes-troubleshooting/kubernetes-oomkilled-error-how-to-fix-and-tips-for-preventing-it/