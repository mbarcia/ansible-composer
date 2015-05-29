# drupsible-composer
Drupsible role for managing PHP composer tool

It needs to be run as root with something like become:yes in your playbook

>  roles:
>   - { role: drupsible-composer, tags: newrelic, become: yes }
