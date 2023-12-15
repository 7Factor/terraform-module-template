# Using this repository as a template

## Naming your repository

When creating a new repository based on this template, you should name it `terraform-<provider>-<module-name>`. For
example, if you were creating a module for creating an S3 bucket, you would name your repository something like
`terraform-aws-s3-bucket`.

After creating a repository based on this template you will need to do the following steps manually:

## Creating labels

Go to the Issues page for your new repository and create the following labels:
* `no release`
* `release:major`
* `release:minor`
* `release:patch`

These labels are required for the release workflow to work properly.

## Creating an initial release

Once you have a basic working module, you will need to manually create an initial v1.0.0 release by tagging a commit
with `v1.0.0` and pushing it to the repository. Then you can create a new release in GitHub using this tag. The release
name should be `Release 1.0.0` assuming the initial version is 1.0.0.

## Adding to the Terraform Registry

After you have an initial release available, you will need to add your module to the Terraform Registry. Simply follow
[this link](https://registry.terraform.io/github/create) and log in with your GitHub account. Then just select the new
repository, agree to the terms, and click "Publish module".

## Updating the README

You will need to update the README to reflect the new module. Remove
[this section](#using-this-repository-as-a-template) and update the remaining sections to reflect the new module.

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
