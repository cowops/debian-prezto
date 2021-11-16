Debian-Prezto
=============

Instantly Awesome Zsh

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

prezto:
    prompt: cloud
    users:
      - vagrant

Dependencies
------------

- cowops.debian_users

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cowops.debian-prezto, debian.users: vagrant }

Tasks
-----

  - Install [prezto](https://github.com/sorin-ionescu/prezto) with a cloud prompt for all {{ prezto.users }}

License
-------

BSD
