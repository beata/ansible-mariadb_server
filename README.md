## [![DebOps project](http://debops.org/images/debops-small.png)](http://debops.org) mariadb_server

[![Travis CI](http://img.shields.io/travis/debops/ansible-mariadb_server.svg?style=flat)](http://travis-ci.org/debops/ansible-mariadb_server) [![test-suite](http://img.shields.io/badge/test--suite-ansible--mariadb__server-blue.svg?style=flat)](https://github.com/debops/test-suite/tree/master/ansible-mariadb_server/)  [![Ansible Galaxy](http://img.shields.io/badge/galaxy-debops.mariadb__server-660198.svg?style=flat)](https://galaxy.ansible.com/list#/roles/4187)

[MariaDB](http://mariadb.org/) is a popular relational SQL database that
was forked from MySQL server. Ansible roles `debops.mariadb` and
`debops.mariadb_server` allow you to manage a MariaDB server and / or
access it remotely from other hosts.

`debops.mariadb_server` role is the "server" part - it installs
`mariadb-server` Debian package, and configures access to the database from
local `root` account. After that, you can use `debops.mariadb` role to
manage databases and user accounts on the server.

### Installation

This role requires at least Ansible `v1.8.0`. To install it, run:

    ansible-galaxy install debops.mariadb_server

### Documentation

More information about `debops.mariadb_server` can be found in the
[official debops.mariadb_server documentation](http://docs.debops.org/en/latest/ansible/roles/ansible-mariadb_server/docs/).


### Role dependencies

- `debops.ferm`
- `debops.secret`
- `debops.tcpwrappers`

### Are you using this as a standalone role without DebOps?

You may need to include missing roles from the [DebOps common
playbook](https://github.com/debops/debops-playbooks/blob/master/playbooks/common.yml)
into your playbook.

[Try DebOps now](https://github.com/debops/debops) for a complete solution to run your Debian-based infrastructure.





### Authors and license

`mariadb_server` role was written by:
- Maciej Delmanowski | [e-mail](mailto:drybjed@gmail.com) | [Twitter](https://twitter.com/drybjed) | [GitHub](https://github.com/drybjed)

License: [GPLv3](https://tldrlegal.com/license/gnu-general-public-license-v3-%28gpl-3%29)

***

This role is part of the [DebOps](http://debops.org/) project. README generated by [ansigenome](https://github.com/nickjj/ansigenome/).
