# Module Name

A basic description of the module and why you would use it.

## Prerequisites

First, you need a decent understanding of how to use Terraform. [Hit the docs](https://www.terraform.io/intro/index.html) for that.

Additional Prereqs

## Example Usage

```hcl-terraform
module "my_module" {
  source  = "7Factor/module-name/aws"
  version = "~> 1"

  some_var = var.some_var
}
```
