Ansible Role: tamay.wildfly
=========

This role installs [WildFly](https://wildfly.org/) application server.

The wildfly process will be run as a systemd service as the user "wildfly".

Requirements
------------

None.

Role Variables
--------------

    # Version as listed in https://wildfly.org/downloads/
    wildfly_version: 16.0.0.Final

WildFly version which will be installed.

    # Mode to run (standalone or domain)
    wildfly_mode: standalone

Choose in which mode wildfly will be run.

Dependencies
------------

None.

Example Playbook
----------------

    ---
    
    - hosts: all
    
      vars:
        wildfly_version: 15.0.1.Final
    
      roles:
      - tamay.wildfly

License
-------

MIT

Author Information
------------------

tamay.mueller@gmail.com
