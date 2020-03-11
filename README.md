# dellemc-powermax-collection
Ansible Galaxy Collection for PowerMax Ansible Modules 1.1

This is a modified version of the official Ansible Modules to be installed as a collection.

Using a collection simplifies the install and managment of modules. 

ansible-galaxy collection install dellemc-powermax-1.1.tar.gz -p ~/.ansible/collections

ansible-doc dellemc.powermax.dellemc_powermax_gatherfacts

To use the collection in a playbook

---
- name: Provisioning storage for Powermax
  hosts: localhost
  connection: local
  gather_facts: no
  collections:
      - dellemc.powermax

All other tasks are as normal.

