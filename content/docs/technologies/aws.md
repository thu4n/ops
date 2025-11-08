---
title: AWS
type: docs
sidebar:
  open: true
---

## AWS CLI Commands

### Get caller identity

```bash
aws sts get-caller-identity
```

Useful for verifying which user/role you are authenticated as.

### Test IAM permissions

```bash
aws iam simulate-principal-policy \
    --policy-source-arn arn:aws:iam::123456789012:user/MyUser \
    --action-names "s3:GetObject" "s3:ListBucket" \
    --resource-arns "arn:aws:s3:::my-bucket/my-file.txt" "arn:aws:s3:::my-bucket"
```

The output will show each action's result (`allowed`, `implicitDeny`, or `explicitDeny`)

### Update kubeconfig to connect to EKS cluster

```bash
aws eks update-kubeconfig --name <cluster-name> --region <region-code>
```

### Others

- https://docs.aws.amazon.com/cli/latest/
