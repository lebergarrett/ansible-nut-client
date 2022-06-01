ansible_nut_client
=========

Ansible role that installs and configures Network Uptime Tools client. Only supports debian-based distros at the moment.

Requirements
------------

You will need to have nut-server installed and set up somewhere already.

Role Variables
--------------

- nut_server_group
- nut_server
- nut_user
- nut_password

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
        - lebergarrett.ansible_nut_client
          vars:
            nut_server_group: tripplite
            nut_server: nut-server.example.com
            nut_user: user
            nut_password: secret # this should be in a vault or passed in at runtime

License
-------

BSD
