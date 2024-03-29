CPU
=========

CPU configuration
It enable cpu governor and set it to `performance` mode. It disables C-State using next options in bootloader:

- processor.max_cstate=0
- intel_idle.max_cstate=0

Requirements
------------

Supports only GRUB options

Role Variables
--------------

No variables

Dependencies
------------

No dependencies

