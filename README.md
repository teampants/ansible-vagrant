[![License](http://img.shields.io/:license-apache-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)
[![Build Status](https://travis-ci.org/teampants/ansible-vagrant.svg?branch=master)](https://travis-ci.org/teampants/ansible-vagrant)
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
