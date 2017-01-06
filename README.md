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

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: loranger.debian-prezto, prezto.users: vagrant }

Tasks
-----

  - Install [prezto](https://github.com/loranger/prezto) with a cloud prompt for all {{ prezto.users }}

License
-------

BSD
