ansible-role-tower-inventory-read-variable
=========

Ansible galaxy role to read variables from an Ansible Tower Inventory.

Requirements
------------

This role assumes that you have a working Ansible Tower environment with credentials.

Role Variables
--------------

tower_hostname: hostname of the Tower server
tower_username: username for Tower
tower_password: password for Tower
inventory_name: name of the inventory within Tower that you want to read variables from.


Usage
----------------

    - hosts: localhost
      roles:
        - role: oatakan.tower-inventory-read-variables
          inventory_name: poc-a-patching

