ansible-role-openwrt-storage
============================

[![Ansible Role: bit_kitchen.openwrt_storage](https://img.shields.io/ansible/role/47608.svg)](https://galaxy.ansible.com/bit_kitchen/openwrt_storage)
[![Build Status: bit-kitchen/ansible-role-openwrt-storage](https://travis-ci.org/bit-kitchen/ansible-role-openwrt-storage.svg?branch=master)](https://travis-ci.org/bit-kitchen/ansible-role-openwrt-storage)

```sh
ansible-galaxy install bit_kitchen.openwrt_storage
```

Configure OpenWrt for USB drive support and auto mount.

Requirements
------------

None.

Role Variables
--------------

Variable   | Default | Comment
---------- | ------- | -------
anon_swap  | yes     | Anonymous Swap: Mount swap not specifically configured
anon_mount | yes     | Anonymous Mount: Mount filesystems not specifically configured
auto_swap  | yes     | Automount Swap: Automatically mount swap on hotplug
auto_mount | yes     | Automount Filesystem: Automatically mount filesystems on hotplug

Dependencies
------------

* `gekmihesg.openwrt`

Example Playbook
----------------

```yml
- hosts: openwrt
  remote_user: root
  gather_facts: no
  roles:
  - bit_kitchen.openwrt_storage
```

License
-------

[MIT](LICENSE)

Author Information
------------------

[bit.kitchen](https://github.com/bit-kitchen)
