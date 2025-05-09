---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "grafana_cloud_access_policies Data Source - terraform-provider-grafana"
subcategory: "Cloud"
description: |-
  Fetches access policies from Grafana Cloud.
  Official documentation https://grafana.com/docs/grafana-cloud/security-and-account-management/authentication-and-permissions/access-policies/API documentation https://grafana.com/docs/grafana-cloud/developer-resources/api-reference/cloud-api/#list-access-policies
  Required access policy scopes:
  accesspolicies:read
---

# grafana_cloud_access_policies (Data Source)

Fetches access policies from Grafana Cloud.

* [Official documentation](https://grafana.com/docs/grafana-cloud/security-and-account-management/authentication-and-permissions/access-policies/)
* [API documentation](https://grafana.com/docs/grafana-cloud/developer-resources/api-reference/cloud-api/#list-access-policies)

Required access policy scopes:

* accesspolicies:read



<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- `name_filter` (String) If set, only access policies with the specified name will be returned. This is faster than filtering in Terraform.
- `region_filter` (String) If set, only access policies in the specified region will be returned. This is faster than filtering in Terraform.

### Read-Only

- `access_policies` (Set of Object) (see [below for nested schema](#nestedatt--access_policies))
- `id` (String) The ID of this datasource. This is an internal identifier used by the provider to track this datasource.

<a id="nestedatt--access_policies"></a>
### Nested Schema for `access_policies`

Read-Only:

- `display_name` (String)
- `id` (String)
- `name` (String)
- `region` (String)
- `status` (String)
