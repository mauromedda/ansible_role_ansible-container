ansible_role_ansible-container
======================

This is a simple ansible role to install ansible-container into a RedHat-like 7+ box.


Requirements
------------

  - Python2
  - Python pip


Example Playbook
----------------

```yaml
---
- hosts: localhost
  become: true
  connection: local

  roles:
    - mauromedda.ansible_role_pip
    - mauromedda.ansible_role_ansible-container
```

Usage
-----

$ ansible-galaxy install -r requirements.yml -p ./roles
$ ansible-playbook -i "localhost," playbook.yml

License
-------

BSD

Author Information
------------------

Author: Mauro Medda 
