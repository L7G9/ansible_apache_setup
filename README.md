# ansible_apache_setup
Install apache2 and configure ufw on ubuntu using ansible
## Description
Ansible playbook to install, configure and run Apache on Unbuntu and configure UFW for use qith Apache.  
## Usage

- Update hosts file.
- Update apache/templates/index.j2.  
- Run apachesetup.yml using:
```
ansible-playbook apachesetup.yml
```
### Author Information
lukewgregory@gmail.com
