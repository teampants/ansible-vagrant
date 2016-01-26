# ansible-vagrant
Basic template-based launch and control of Vagrant VMs

## Prerequisites
Vagrant must be installed on your ansible system.

## Example Playbook

~~~
- hosts: local-vagrant
  gather_facts: false
  roles:
    - role: teampants.vagrant
~~~
