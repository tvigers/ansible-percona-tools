Percona Tools
=========

[![Travis](https://travis-ci.org/tvigers/ansible-percona-tools.svg?branch=master)](https://travis-ci.org/tvigers/ansible-percona-tools)

Simple role to managed the installation of Percona Toolkit and Percona xtrabackup.

Role Variables
--------------

The below manages installation of the Percona packages:

    percona_toolkit_packages:
      - percona-toolkit
      - percona-xtrabackup-24

Sets the source of the Percona YUM repo:

    percona_yum_repository: 'https://repo.percona.com/yum/percona-release-latest.noarch.rpm'

Dependencies
------------

N/A

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: ansible-percona-tools }

License
-------

Apache

Author Information
------------------

Timothy Vigers (tvigers@serversumo.io)
