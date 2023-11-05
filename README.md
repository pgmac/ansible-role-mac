Role Name
=========

This is a collection of tasks to help manage my MacBook setup

Requirements
------------

Homebrew. But, this should get installed by this role, too.

Role Variables
--------------

| Variable    | Description                                                                                           |
| ----------- | ----------------------------------------------------------------------------------------------------- |
| user_shell  | Which shell do you prefer? `bash` or `zsh`                                                            |
| kill_my_mac | !!Dangerious variable!! Only to be used when you need to clean your MacBook and remove all your stuff |

Dependencies
------------

Example Playbook
----------------

Installing some base/common stuff and setting your shell to 'zsh'

    - hosts: localhost
      roles:
         - { role: ansibole-role-mac, user_shell: zsh }


Killing everything you have on your Mac

    - hosts: localhost
      roles:
         - { role: ansibole-role-mac, user_shell: zsh, kill_my_mac: true }


License
-------

BSD

Author Information
------------------

Paul Macdonnell
pgmac@pgmac.net
https://www.pgmac.net.au
https://github.com/pgmac/ansible-role-mac
