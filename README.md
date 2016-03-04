drupsible-composer
==================

Provides Composer (https://getcomposer.org/). It makes the 'composer' command available globally in the system.

Requirements
------------

PHP installed and available globally as a command "php".

This role can be used indepedently and does NOT require Drupsible to run.

Example Playbook
----------------

```
- role: drupsible.composer
  become: yes
  tags: [ 'role::composer' ]
```

License
-------

GNU General Public License v3

Author Information
------------------

Mariano Barcia - [https://github.com/mbarcia](https://github.com/mbarcia)
