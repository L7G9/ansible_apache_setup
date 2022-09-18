ufw
=========
A role to configure UFW for use with Apache.  Also configures UFW so Ansible can continue to be used on host after UFW is started.  

Requirements
------------
Ansible UFW module.  
Check if this is installed with:
```
$ ansible-doc -l
```

Install with:
```
$ ansible-galaxy collection install community.general
```

Role Variables
--------------
None.

Dependencies
------------
None.

Example Playbook
----------------

```
---
- name: set up ufw for apache on webservers
  hosts: web_servers
  become: yes
  roles:
    - ufw
```

Author Information
------------------
lukewgregory@gmail.com
