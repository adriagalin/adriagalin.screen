adriagalin.screen
=================

[![Build Status](https://travis-ci.org/adriagalin/ansible.screen.svg?branch=master)](https://travis-ci.org/adriagalin/ansible.screen) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-screen-blue.svg)](https://galaxy.ansible.com/adriagalin/screen)

An ansible role for configuring screen.

Requirements
------------

Tested on:

-	>= Ubuntu 16.04 LTS

Should work with:

-	All Ubuntu
-	All Debian

Role Variables
--------------

```yaml
ag_screen_startup_message: enable/disable screen startup message

ag_screenrc_destinations:
  current:
    dest: "{{ ansible_env.HOME }}"
  vagrant:
    dest: /home/vagrant
    owner: vagrant
    group: vagrant
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
----

-	Add per user configuration.
-	Add more screen custom configurations.

License
-------

GPLv3 License.

Author Information
------------------

[Adria Galin](http://www.adriagalin.com)

Inspiration
-----------

During development, some roles in Ansible Galaxy/Github also inspired me:

-	[tersmitten](https://github.com/Oefenweb/ansible-screen)

thank you.
