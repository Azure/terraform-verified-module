# Verified Terraform Module

The Verified Terraform module is a template repository to help developers create their own Terraform Module.

Enjoy it by following steps:

1. Use [this template](https://github.com/lonegunmanb/terraform-verified-module) to create your repository.
2. Write Terraform code in a new branch.
3. Run `make pre-commit` to check in local.
4. Create a pull request for the main branch.
    * The title must be a [conventional message](https://www.conventionalcommits.org/)
    * CI check will be executed automatically.
5. Merge pull request, release, and tag will be auto-generated.
6. Enjoy it!

<!-- BEGIN_TF_DOCS -->
## Requirements

No requirements.

## Providers

No providers.

## Modules

No modules.

## Resources

No resources.

## Inputs

| Name                                           | Description   | Type     | Default | Required |
|------------------------------------------------|---------------|----------|---------|:--------:|
| <a name="input_echo"></a> [echo](#input\_echo) | Hello, world! | `string` | n/a     |   yes    |

## Outputs

| Name                                             | Description |
|--------------------------------------------------|-------------|
| <a name="output_echo"></a> [echo](#output\_echo) | n/a         |
<!-- END_TF_DOCS -->
