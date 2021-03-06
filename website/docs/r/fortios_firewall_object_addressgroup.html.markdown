---
layout: "fortios"
page_title: "FortiOS: fortios_firewall_object_addressgroup"
sidebar_current: "docs-fortios-resource-firewall-object-addressgroup"
description: |-
  Provides a resource to configure firewall address group used in firewall policies of FortiOS.
---

# fortios_firewall_object_addressgroup
Provides a resource to configure firewall address group used in firewall policies of FortiOS.

## Example Usage
```hcl
resource "fortios_firewall_object_addressgroup" "s1" {
  name    = "s1"
  member  = ["google-play", "swscan.apple.com"]
  comment = "dfdsad"
}
```

## Argument Reference
The following arguments are supported:

* `name` - (Required) Address group name.
* `member` - (Required) Address objects contained within the group.
* `comment` - Comment.

## Attributes Reference
The following attributes are exported:

* `id` - The ID of the firewall address group item.
* `name` - Address group name.
* `member` - Address objects contained within the group.
* `comment` - Comment.
