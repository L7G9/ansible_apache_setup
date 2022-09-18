apache
=========

A role to install Apache on Ubuntu, configure index.html using a template and start the service.  

Requirements
------------

All modules used by this role are part of ansible-core and included in all Ansible installations.
Template for index.html is stored in templates/index.j2.  

Role Variables
--------------
None

Dependencies
------------

None

Example Playbook
----------------
```
---
- name: set up apache on webservers
  hosts: web_servers
  become: yes
  roles:
    - apache
```

Author Information
------------------

lukewgregory@gmail.com
