# ansible-vagrant
Basic template-based launch and control of Vagrant VMs

## Prerequisites
Vagrant must be installed on your ansible system.

## Adding hosts to /etc/hosts on your local workstastion
To add the created host(s) to your local /etc/hosts set ~vagrant_add_to_local_etc_hosts~ to true.

**Warning: You must set serial=1 on the play that includes this role to use this feature, due to concurrency issues when
editing files. This requirement will go away in the future. See https://github.com/ansible/ansible-modules-core/pull/1902**

## Example Playbook

~~~
- hosts: local-vagrant
  gather_facts: false
  roles:
    - role: teampants.vagrant
~~~
