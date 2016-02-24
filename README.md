Ansible Packer playbook
=====

This role installs or updates Packer on a server.

Requirements
------------

This role requires Ansible 1.4 or higher and platform requirements are listed
in the metadata file.

Role Variables
--------------

The variables that can be passed to this role and a brief description about
them are as follows.

```
# Packer version to install
packer_version: '0.9.0'
packer_arch: 'linux_amd64'
# Packer destination folder
packer_destination: '/usr/bin'
```

Examples
========

```
# Roles
- name: packer
  hosts: packer
  user: root
  roles:
    - packer
  vars:
    - packer_version: '0.9.0'

```

Dependencies
------------

None

License
-------

GPL

Author Information
------------------

Pierre Mavro / deimosfr


