# Network ACL Module Example

This module is used to create a Network ACL

This example illustrates how to use the `network_acl` module

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->

## Inputs

| Name                              | Description                                           | Type   | Default | Required |
|-----------------------------------|-------------------------------------------------------|--------|---------|----------|
| create\_vpc | True to create new VPC.| bool | n/a | yes |
| enable\_acl | True to Enable ACL| bool | true | no |
| resource\_group | Name of the resource group | string | n/a | no |
| name | Name of the Network ACL | string | n/a | yes |
| vpc\_name | Name of the VPC | string | n/a | yes |
| rules | List of Network ACL Rules that are to be attached to the ACL  | object | n/a | no |
| tags | List of tags to attach  | list(string) | n/a | no |


<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->

NOTE: We can configure the rules to be attached to the network_acl by entering respective details in input.tfvars.

## Usage

terraform apply -var-file="input.tfvars"

## Note

For all optional fields, default values (Eg: `null`) are given in varaible.tf file. User can configure the same by overwriting with appropriate values.