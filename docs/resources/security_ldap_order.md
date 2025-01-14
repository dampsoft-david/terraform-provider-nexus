---
page_title: "Resource nexus_security_ldap_order"
subcategory: "Security"
description: |-
  Use this resource to change the LDAP order.
---
# Resource nexus_security_ldap_order
Use this resource to change the LDAP order.
## Example Usage
```terraform
resource "nexus_security_ldap" "server1" {
  ...
  name = "server1"
}

resource "nexus_security_ldap" "server2" {
  ...
  name = "server2"
}

resource "nexus_security_ldap_order" "system" {
  order = [
    nexus_security_ldap.server1.name,
    nexus_security_ldap.server2.name,
  ]
}
```
<!-- schema generated by tfplugindocs -->
## Schema

### Required

- **order** (List of String) Ordered list of LDAP server

### Read-Only

- **id** (String) Used to identify resource at nexus

