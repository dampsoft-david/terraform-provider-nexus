---
page_title: "Data Source nexus_user"
subcategory: "Other"
description: |-
  !> This data source is deprecated. Please use the data source "nexussecurityuser" instead.
  Use this data source to get a user data structure.
---
# Data Source nexus_user
!> This data source is deprecated. Please use the data source "nexus_security_user" instead.

Use this data source to get a user data structure.

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- **userid** (String) The userid which is required for login

### Read-Only

- **email** (String) The email address associated with the user.
- **firstname** (String) The first name of the user.
- **id** (String) Used to identify data source at nexus
- **lastname** (String) The last name of the user.
- **roles** (Set of String) The roles which the user has been assigned within Nexus.
- **status** (String) The user's status, e.g. active or disabled.

