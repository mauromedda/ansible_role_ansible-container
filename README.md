ansible_role_ansible-container
======================

This is a simple ansible role to install ansible-container into a RedHat-like 7+ box.


Requirements
------------

  - Python2
  - Python pip


Variables
---------

Look for the variable in [`defaults/main.yml`](defaults/main.yml)


  * container_engine: "docker"

Ansible Container relies upon supported container engines for building, running, and deploying your project.
When you install Ansible Container, you must specify which engines you want your installation to support.
Currently supported engines are:
  - docker
  - k8s
  - openshift.


Example Playbook
----------------

```yaml
---
- hosts: localhost
  become: true
  connection: local

  roles:
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
