adriagalin.screen
=========

[![Build Status](https://travis-ci.org/adriagalin/ansible.screen.svg?branch=master)](https://travis-ci.org/adriagalin/ansible.screen) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-screen-blue.svg)](https://galaxy.ansible.com/list#/roles/4778)

An ansible role for configuring screen.

Requirements
------------

Tested on:

Ubuntu 14.04 LTS

Should work with:

All Ubuntu
All Debian

Role Variables
--------------

```yaml
ag_screen_startup_message: enable/disable screen startup message
```

Dependencies
------------

None.

Example Playbook
----------------
```yaml
    - hosts: servers
      roles:
         - { role: adriagalin.screen }
```

ToDo
-------
- Add per user configuration.
- Add more screen custom configurations.

License
-------

GPLv3 License.

Author Information
------------------

[Adrià Galín](http://www.adriagalin.com)

Inspiration
------------------

During development, some roles in Ansible Galaxy/Github also inspired me:

  - [tersmitten](https://github.com/Oefenweb/ansible-screen)

  thank you.
