---
title: Terraform
type: docs
sidebar:
  open: true
---

## `moved` block

The `moved` block in Terraform allows you to rename a `resource` or `module` without destroying and recreating it. This is useful when you want to change the name of a resource in your configuration to better reflect its purpose, but you want to preserve the state of the existing resource.

### Example

To rename a resource from `aws_instance.old_name` to `aws_instance.new_name`, you would add the following `moved` block to your configuration:

```terraform
moved {
  from = aws_instance.old_name
  to   = aws_instance.new_name
}
```

After adding the `moved` block, you can safely rename the resource in your configuration file. When you run `terraform apply`, Terraform will recognize the change and update the state file accordingly, without destroying the existing EC2 instance.
