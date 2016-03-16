mariadb
=========

Ansible role to install mariadb

Requirements
------------

No further requirements besides bash.

Role Variables
--------------

{{ mariadb.user }}
{{ mariadb.root_password }}
{{ mariadb.database }}

Dependencies
------------

No dependencies.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: bytepark.mariadb }

License
-------

MIT

Author Information
------------------

bytepark / 2016.
