ufw
=========

A role to configure UFW for use with Apache.  Also configures UFW so Ansible can continue to be used on host after UFW is started.  

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

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
