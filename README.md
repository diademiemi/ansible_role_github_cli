Ansible Role Template
=========

This is an Ansible role to install and configure github_cli.

This role uses the GitHub CLI mirrors to install the packages on supported platforms, it does need any variables to be set.

Requirements
------------
These platforms are supported:
- Ubuntu 20.04  
- Ubuntu 22.04  
- Debian 10  
- Debian 11  
- EL 8 (Tested on Rocky Linux 8)  
- EL 9 (Tested on Rocky Linux 9)  
- Fedora 38  

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
- name: Use github_cli role
  hosts: "{{ target | default('github_cli') }}"
  roles:
    - diademiemi.github_cli
```

License
-------

MIT

Author Information
------------------

- diademiemi (@diademiemi)

Role Testing
------------

This repository comes with Molecule tests for Docker on the supported platforms.
Install Molecule by running
```bash
pip3 install -r requirements.txt
```

Run the tests with
```bash
molecule test
```
