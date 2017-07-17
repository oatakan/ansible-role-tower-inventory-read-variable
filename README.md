ansible-role-tower-inventory-read-variable
=========

Ansible galaxy role to read variables from an Ansible Tower Inventory.

Requirements
------------

This role assumes that you have a working Ansible Tower environment with credentials.

Role Variables
--------------

**tower_hostname:** hostname of the Tower server

**tower_username:** username for Tower

**tower_password:** password for Tower

**inventory_name:** name of the inventory within Tower that you want to write variables to. If this inventory doesn't exists it will be created.

**inventory_variables:** variable holding dict of other variables that are read from the inventory


Usage
----------------

    - hosts: localhost
      roles:
        - role: oatakan.tower-inventory-read-variable
          inventory_name: poc-a-patching

