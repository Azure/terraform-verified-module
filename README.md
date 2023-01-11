# Verified Terraform Module

The Verified Terraform module is a template repository to help developers create their own Terraform Module.

Enjoy it by following steps:

1. Use [this template](https://github.com/Azure/terraform-verified-module) to create your repository.
2. Write Terraform code in a new branch.
3. Update [`acc-test.yaml`](.github/workflows/acc-test.yaml), modify `runs-on: [self-hosted, 1ES.Pool=<YOUR_REPO_NAME>]` with your 1es runners' pool name (basically it's your repo's name).
4. Run `docker run --rm -v $(pwd):/src -w /src mcr.microsoft.com/azterraform:latest make pre-commit` to format the code. On PowerShell, run `docker run --rm -v ${pwd}:/src -w /src mcr.microsoft.com/azterraform:latest make pre-commit`.
5. Run `docker run --rm -v $(pwd):/src -w /src mcr.microsoft.com/azterraform:latest make pr-check` to run the check in local. On PowerShell, run `docker run --rm -v ${pwd}:/src -w /src mcr.microsoft.com/azterraform:latest make pr-check`.
6. Create a pull request for the main branch.
    * CI pr-check will be executed automatically.
    * Once pr-check was passed, with manually approval, the e2e test and version upgrade test would be executed.
7. Merge pull request.
8. Enjoy it!

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
