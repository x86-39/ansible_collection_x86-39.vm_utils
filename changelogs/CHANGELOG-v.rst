=================================
diademiemi.vm_utils Release Notes
=================================

.. contents:: Topics


v3.0.0
======

Release Summary
---------------

This release adds workspace support to terraform playbooks. It also requires my fork of cloud.terraform collection.

Major Changes
-------------

- add workspace support in terraform playbooks

Breaking Changes / Porting Guide
--------------------------------

- now requires my fork of cloud.terraform collection
- workspace now defaults to provider-env, instead of "default"

v2.0.0
======

Release Summary
---------------

This release is a major overhaul of the terraform_vms playbook. It is now much more flexible and can be used to create and destroy VMs in a much more dynamic way.

Major Changes
-------------

- Added new playbook terraform_dns for changing DNS records through Ansible w/ Terraform
- Added new playbook terraform_inv_mgt for changing inventory sources
- Rewrote terraform_vms playbook, CHECK NEW DOCUMENTATION

v1.0.0
======

Release Summary
---------------

initial release

Major Changes
-------------

- add terraform_vms playbook
- add vyos_qcow2_image role
