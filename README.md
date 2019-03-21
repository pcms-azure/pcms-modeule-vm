# pcms-module-vm

Module for an individual VM with cloud-init

Initial version copied manually from <https://github.com/Azure/terraform-azurerm-compute>.

Changes:

* Removed windows
* Removed boot diagnostics
* Removed sub-module
* Use existing resource group and subnet
* Use location and tags from resource group if unspecified (tags always pulled, but can be overridden)
* Only one nic, max one pip plus dns
* Simplified names
* Fixed to PCMS project and environment_name