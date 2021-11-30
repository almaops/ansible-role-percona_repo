Role Name
=========

Ansible role to configure [Percona Software repositories](https://www.percona.com/doc/percona-repo-config/index.html).  

Requirements
------------

Currently only Debian-based distributions are supported

Role Variables
--------------

|Name|Default value|Description|
|----|-------------|-----------|
|`percona_repo_url`|`https://repo.percona.com/apt/percona-release_latest.generic_all.deb`|Link to `percona-release` deb package|
|`percona_repo_configure`|`false`|Whether to run `percona-release`|
|`percona_repo_release`|`show`|Arguments for `percona-release`|

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
           percona_repo_release: "enable ps-80 release"

License
-------

[MIT](./LICENSE)
