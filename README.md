ansible-ntp
===========

Set up *ntp service* + *time zone* on RHEL/CentOS and Debian/Ubuntu.

Requirements
------------

None.

Role Variables
--------------

    time_zone: Anctartica/South_Pole  # time zone, must exist under `/usr/share/zoneinfo/`

    ntp_servers:
      - 0.pool.ntp.org
      - 1.pool.ntp.org
      - 2.pool.ntp.org
      - 3.pool.ntp.org


Dependencies
------------

None.

Example Playbook
-------------------------

    - hosts: all
      sudo: true
      vars:
        time_zone: Europe/Berlin
      roles:
        - ntp

License
-------

MIT

Author Information
------------------

José Fernández Ramos <el.atomo@gmail.com>
