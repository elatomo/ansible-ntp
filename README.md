ansible-ntp
===========

Set up *ntp service* + *time zone*.

Requirements
------------

None.

Role Variables
--------------

    time_zone: Anctartica/South_Pole  # time zone, must exist under `/usr/share/zoneinfo/`.


Dependencies
------------

None.

Example Playbook
-------------------------

    - hosts: all
      sudo: true
      roles:
         - ntp

License
-------

MIT

Author Information
------------------

José Fernández Ramos <el.atomo@gmail.com>
