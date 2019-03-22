Ansible Plug-in for `systemd-escape`
=========

An Ansible plug-in which uses `systemd-escape` to manipulate strings for use in systemd units.

Requirements
------------

You'll need to have a recent-ish version of systemd on the host where the filer will be running.

Example Playbook
----------------

    - hosts: servers
      roles:
        - ansible-plugin-systemd_escape
      tasks:
        - debug: msg={{ "Hello, World!" | systemd_escape }}

License
-------

GPLv3

Author Information
------------------

* Estelle Poulin <dev@inspiredby.es>
