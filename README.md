[![Build Status](https://travis-ci.org/bytepark/ansible-role-mariadb.svg?branch=master)](https://travis-ci.org/bytepark/ansible-role-mariadb)

ansible-role-mariadb
=========

Ansible role to install mariadb

Requirements
------------

No further requirements

Role Variables
--------------

Available variables are listed below, along with default values:

	# Users and init config
	mariadb_user_home: /root
	mariadb_root_user: root
	mariadb_root_password: rootpassword
	mariadb_user: mariadb
	mariadb_password: mariadbpassword
	mariadb_database: mariadb
	mariadb_upstream_version: 10.1
	mysql_enabled_on_startup: yes

	# Set this to `yes` to forcibly update the root password.
	mariadb_root_password_update: no

	# Databases.
	mysql_databases: []
	#   - name: example
	#     collation: utf8_general_ci
	#     encoding: utf8
	#     replicate: 1

	# Users.
	mysql_users: []
	#   - name: example
	#     host: 127.0.0.1
	#     password: secret
	#     priv: *.*:USAGE


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
