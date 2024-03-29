Network
=========

Network configuration for new servers
It renames default interface to `net0`

Requirements
------------

Supports only Ubuntu releases (with netplan)

Role Variables
--------------

`mac_address` - macaddress of the default interface. Default: `ansible_facts['default_ipv4']['macaddress']`

Dependencies
------------

No dependencies

