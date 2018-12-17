## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| attributes | Additional attributes (e.g. `1`) | list | `<list>` | no |
| cluster_name | Kops cluster name (e.g. `us-east-1.cloudposse.co` or `cluster-1.cloudposse.co`) | string | - | yes |
| delimiter | Delimiter to be used between `namespace`, `stage`, `name` and `attributes` | string | `-` | no |
| masters_name | Kops masters subdomain name in the cluster DNS zone | string | `masters` | no |
| name | Name (e.g. `atlantis`) | string | `atlantis` | no |
| namespace | Namespace (e.g. `eg` or `example`) | string | - | yes |
| nodes_name | Kops nodes subdomain name in the cluster DNS zone | string | `nodes` | no |
| policy_arn | Permission to grant to atlantis server | string | `arn:aws:iam::aws:policy/AdministratorAccess` | no |
| stage | Stage (e.g. `prod`, `dev`, `staging`) | string | - | yes |
| tags | Additional tags (e.g. map(`Cluster`,`us-east-1.cloudposse.co`) | map | `<map>` | no |

## Outputs

| Name | Description |
|------|-------------|
| policy_arn | IAM policy ARN |
| role_arn | IAM role ARN |
| role_name | IAM role name |
| role_unique_id | IAM role unique ID |

