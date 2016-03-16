Role Name
=========

Ansible role to install mariadb

Requirements
------------

No further requirements

Role Variables
--------------

Available variables are listed below, along with default values:

	mariadb_user: mariadb
	mariadb_password: mariadbpassword
	mariadb_root_password: rootpassword
	mariadb_database: mariadb

Dependencies
------------

No dependencies

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: bytepark.mariadb }
      vars:
      	mariadb_user: mariadb
	  	mariadb_password: mariadbpassword
		mariadb_root_password: rootpassword
		mariadb_database: mariadb

License
-------

MIT

Author Information
------------------

bytepark / 2016.
