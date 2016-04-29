drupsible-composer
==================

Provides Composer (https://getcomposer.org/). It makes the 'composer' command available globally in the system.

Requirements
------------

PHP installed and available globally as a command "php".

This role can be used indepedently and does NOT require Drupsible to run.

Example Playbook (latest installer, version 1.0.0 of composer)
---------------------------------------------

```
- role: drupsible.composer
  composer_installer_url: "https://getcomposer.org/installer"
  composer_installer_checksum_enabled: no
  composer_version_latest_enabled: no 
  composer_version: "--version=1.0.0" 
  become: yes
  tags: [ 'role::composer' ]
```

Example Playbook (latest installer and latest version of composer)
---------------------------------------------

```
- role: drupsible.composer
  composer_installer_url: "https://getcomposer.org/installer"
  composer_installer_checksum_enabled: no
  become: yes
  tags: [ 'role::composer' ]
```

Example Playbook (installer with checksum of 28/4/2016, and latest version of composer)
---------------------------------------------

```
- role: drupsible.composer
  become: yes
  tags: [ 'role::composer' ]
```

You can also specify ``composer_installer_url`` and ``composer_installer_checksum`` if you want a specific or updated version of the installer/setup PHP script.

License
-------

GNU General Public License v3

Author Information
------------------

Mariano Barcia - [https://github.com/mbarcia](https://github.com/mbarcia)
