Lacework Ansible Role
=========

Ansible Role to deploy the Lacework server agent.

Platforms
---------

* Ubuntu
* CentOS
* RedHat

Role Variables
--------------
The following variables are available for override.

```
lacework_accessToken:         # Required. Your Lacework access token.
```

Install
----------------
Using ansible galaxy, best for ad-hoc command situations:

    $ ansible-galaxy install lacework.lacework-ansible

To install into your playbook roles, use `-p ROLES_PATH` or `--path=ROLES_PATH`

    $ ansible-galaxy install lacework.lacework-ansible -p /your/project/root/roles

Check out: [Advanced Control over Role Requirements Files](http://docs.ansible.com/galaxy.html#advanced-control-over-role-requirements-files)


Examples
----------------
1) Install Lacework agent.
```
- hosts: all
  roles:
    - { role: lacework.lacework-ansible, lacework_accessToken: XXXXXXXXXXXXX}
```

Dependencies
------------

None

License
-------

Mozilla Public License Version 2.0

Author Information
------------------
matthew zeier <mzeier@gmail.com>
Use github issues for bugs in this repo.

