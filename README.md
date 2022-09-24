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

| Name                                                                      | Version |
|---------------------------------------------------------------------------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 1.2  |
| <a name="requirement_null"></a> [null](#requirement\_null)                | >= 3.1  |

## Providers

| Name                                                 | Version |
|------------------------------------------------------|---------|
| <a name="provider_null"></a> [null](#provider\_null) | >= 3.1  |

## Modules

No modules.

## Resources

| Name                                                                                                       | Type     |
|------------------------------------------------------------------------------------------------------------|----------|
| [null_resource.nop](https://registry.terraform.io/providers/hashicorp/null/latest/docs/resources/resource) | resource |

## Inputs

| Name                                                            | Description      | Type     | Default | Required |
|-----------------------------------------------------------------|------------------|----------|---------|:--------:|
| <a name="input_echo_text"></a> [echo\_text](#input\_echo\_text) | The text to echo | `string` | n/a     |   yes    |

## Outputs

| Name                                                              | Description      |
|-------------------------------------------------------------------|------------------|
| <a name="output_echo_text"></a> [echo\_text](#output\_echo\_text) | The text to echo |
<!-- END_TF_DOCS -->
