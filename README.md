<!-- BEGIN_TF_DOCS -->
## Module Docs
### Examples

```hcl

```
----
### Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_github_organisation_name"></a> [github\_organisation\_name](#input\_github\_organisation\_name) | TODO | `string` | n/a | yes |
| <a name="input_github_url"></a> [github\_url](#input\_github\_url) | TODO | `string` | n/a | yes |
| <a name="input_iam_instance_profile_arn"></a> [iam\_instance\_profile\_arn](#input\_iam\_instance\_profile\_arn) | TODO | `string` | n/a | yes |
| <a name="input_instance_type"></a> [instance\_type](#input\_instance\_type) | TODO | `string` | n/a | yes |
| <a name="input_naming_prefix"></a> [naming\_prefix](#input\_naming\_prefix) | TODO | `string` | n/a | yes |
| <a name="input_region"></a> [region](#input\_region) | TODO | `string` | n/a | yes |
| <a name="input_spot_price"></a> [spot\_price](#input\_spot\_price) | TODO | `string` | n/a | yes |
| <a name="input_ssh_authorized_keys"></a> [ssh\_authorized\_keys](#input\_ssh\_authorized\_keys) | TODO | `list(string)` | `[]` | no |
| <a name="input_ssm_parameter_name"></a> [ssm\_parameter\_name](#input\_ssm\_parameter\_name) | TODO | `string` | `"/github/runner/token"` | no |
| <a name="input_subnet_ids"></a> [subnet\_ids](#input\_subnet\_ids) | TODO | `list(string)` | n/a | yes |
| <a name="input_vpc_id"></a> [vpc\_id](#input\_vpc\_id) | TODO | `string` | n/a | yes |
----
### Modules

No modules.
----
### Outputs

No outputs.
----
### Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | 4.27.0 |
| <a name="provider_http"></a> [http](#provider\_http) | 3.0.1 |
----
### Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 0.13.1 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | >= 4.9 |
| <a name="requirement_http"></a> [http](#requirement\_http) | 3.0.1 |
----
### Resources

| Name | Type |
|------|------|
| [aws_autoscaling_group.runners](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/autoscaling_group) | resource |
| [aws_autoscaling_policy.runners_scale_down](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/autoscaling_policy) | resource |
| [aws_cloudwatch_metric_alarm.runners_scale_down](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_metric_alarm) | resource |
| [aws_launch_configuration.runners](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/launch_configuration) | resource |
| [aws_security_group.runners_ec2](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) | resource |
| [aws_security_group_rule.ingress](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group_rule) | resource |
| [aws_ami.ami](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/ami) | data source |
| [aws_ssm_parameter.runner](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/ssm_parameter) | data source |
| [http_http.myip](https://registry.terraform.io/providers/hashicorp/http/3.0.1/docs/data-sources/http) | data source |
----
```
<!-- END_TF_DOCS -->