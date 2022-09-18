ufw
=========
A role to configure UFW for use with Apache.  Also configures UFW so Ansible can continue to be used on host after UFW is started.  

Requirements
------------
Ansible UFW module.  
You can check if this is installed with...
'$ ansible-doc -l'

Then install if required...
'$ ansible-galaxy collection install community.general'

Role Variables
--------------
None.

Dependencies
------------
None.

Example Playbook
----------------
---
- name: set up ufw for apache on webservers
  hosts: web_servers
  become: yes
  roles:
    - ufw

Author Information
------------------
lukewgregory@gmail.com
