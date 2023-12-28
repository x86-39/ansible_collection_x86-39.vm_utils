Ansible Collection - diademiemi.vm_utils
========================================
Documentation for the collection vm_utils.

Contents 
========

Roles
------
Role | Description | CI Status
--- | --- | ---
[diademiemi.vm_utils.vyos_qcow2_image](./roles/vyos_qcow2_image/) | Compile VyOS cloud image with Cloud Init installed | N/A
<!-- [diademiemi.vm_utils.EXAMPLE](./roles/vm_utils/) | Install EXAMPLE | [![Molecule test](https://github.com/diademiemi/ansible_collection_diademiemi.vm_utils/actions/workflows/ansible-role-EXAMPLE.yml/badge.svg)](https://github.com/diademiemi/ansible_collection_diademiemi.vm_utils/actions/workflows/ansible-role-EXAMPLE.yml) -->

Playbooks
------
Playbook | Description | CI Status
--- | --- | ---
[diademiemi.vm_utils.terraform_inv_mgt](./playbooks/terraform_inv_mgt.yml) | Set up inventory file for terraform-managed inventory. Should be run on localhost | N/A
[diademiemi.vm_utils.terraform_vms](./playbooks/terraform_vms.yml) | Set up Terraform VMs according to variables & sync hostnames to `/etc/hosts`. Should be run on localhost | N/A
[diademiemi.vm_utils.terraform_dns](./playbooks/terraform_dns.yml) | Set up Terraform DNS with output from terraform_vms.yml. Should be run on localhost | N/A


Click on the role to see the README for that role.  

