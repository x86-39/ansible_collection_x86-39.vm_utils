===============================
x86\_39.vm\_utils Release Notes
===============================

.. contents:: Topics

v8.1.0
======

Release Summary
---------------

New namespace: x86_39

Major Changes
-------------

- Move repo to github.com/x86-39

v8.0.1
======

Bugfixes
--------

- Fix changing remote backend

v8.0.0
======

Release Summary
---------------

Overhaul terraform_remote_backend.yml

Major Changes
-------------

- Add new variables to terraform_remote_backend.yml

v7.0.0
======

Major Changes
-------------

- Allow getting variables from env vars for certain options in playbooks. Check playbook documentation for more information.

v6.1.0
======

Bugfixes
--------

- Fix handler in terraform_remote_backend.yml

v6.0.0
======

Release Summary
---------------

This release adds a new playbook terraform_remote_backend.yml and reworks terraform_inv_mgt.yml

Major Changes
-------------

- Add terraform_remote_backend.yml playbook
- Rework terraform_inv_mgt.yml playbook to place the whole file instead of modifying in place

v5.1.0
======

Release Summary
---------------

Fix handling for subdomains for /etc/hosts

v5.0.0
======

Release Summary
---------------

Complete overhaul of all playbooks

Major Changes
-------------

- Added new variables (check playbook docs)
- Changed default terraform path to /terraform/<purpose>/<provider>
- Changed default tfvars path to /tfvars/<purpose>/<provider>/<env>.tfvars
- Changed variable precedence to prefer shortcuts

v4.1.0
======

Release Summary
---------------

Fix removing hostnames

Bugfixes
--------

- Fix removing hostnames

v4.0.1
======

Release Summary
---------------

Fix vyos compile

Bugfixes
--------

- Fix typo in vyos compile

v4.0.0
======

Release Summary
---------------

Add workspaces support for a smaller setup footprint

Major Changes
-------------

- Add workspaces support
- Change variables, check documentation

v3.1.0
======

Release Summary
---------------

Minor changes to terraform_inv_mgt

Minor Changes
-------------

- Make inventory_path overridable in terraform_inv_mgt
- Update README.md

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
