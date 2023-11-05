Ansible Role Template
=========



This is an Ansible role to install and configure vyos_qcow2_image.

Include more information about vyos_qcow2_image in this section.

Requirements
------------

<!--
- List hardware requirements here  
-->

Role Variables
--------------

Variable | Default | Description
--- | --- | ---
<!--
`variable` | `default` | Variable example
`long_variable` | See [defaults/main.yml](./defaults/main.yml) | Variable referring to defaults
`distro_specific_variable` | See [vars/debian.yml](./vars/debian.yml) | Variable referring to distro-specific variables
-->

Dependencies
------------
<!-- List dependencies on other roles or criteria -->
None

Example Playbook
----------------

```yaml
- name: Use diademiemi.vyos_qcow2_image role
  hosts: "{{ target | default('vyos_qcow2_image') }}"
  roles:
    - role: "diademiemi.vyos_qcow2_image"
      tags: ['diademiemi', 'vyos_qcow2_image', 'setup']    ```

```

License
-------

MIT

Author Information
------------------

- diademiemi (@diademiemi)
