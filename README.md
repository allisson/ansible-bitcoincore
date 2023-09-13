Role Name
=========

Installs bitcoin core using https://raspibolt.org/ as a reference.

Role Variables
--------------

See [defaults/main.yml](defaults/main.yml)

Example Playbook
----------------

```yml
---
- name: Example playbook
  hosts: localhost
  become: yes

  roles:
    - role: allisson.ansible_bitcoincore
      vars:
        version: "25.0"
        bitcoin_user: bitcoin
        bitcoin_group: bitcoin
        bitcoin_uid: 2000
        bitcoin_gid: 2000
        rpc_user: bitcoin
        rpc_password: bitcoin
        enable_tor: true
        optimize_for_raspberrypi: false
        optimize_for_initial_block_download: false
```

License
-------

MIT

Author Information
------------------

[Allisson Azevedo](https://github.com/allisson)
