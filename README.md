# drupsible-composer
## Provides Composer (https://getcomposer.org/)

It needs to be run as root with something like become:yes in your playbook

>  roles:
>   - { role: drupsible.composer, tags: composer, become: yes }

## Requirements
PHP installed and available globally as a command "php".

## Notes
While this role is part of the Drupsible project, it can be used independently.
