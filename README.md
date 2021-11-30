Role Name
=========

Ansible role to configure [Percona Software repositories](https://www.percona.com/doc/percona-repo-config/index.html).  

Requirements
------------

Currently only Debian-based distributions are supported

Role Variables
--------------

None

Dependencies
------------

None

Example Playbook
----------------

As simple as:

    - hosts: mysql_servers
      roles:
         - role: almaops.percona_repo
           percona_repo_configure: true
           percona_repo_product: "ps80"

License
-------

[MIT](./LICENSE)
