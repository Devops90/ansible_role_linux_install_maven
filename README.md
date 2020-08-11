Role Name
=========

Install Apache maven.

Requirements
------------

Ansible version: 2.9   
Operating systems: Amazon-Linux.  
                   Redhat7, Redhat8.

Role Variables
--------------
 
maven_major: 3  
maven_version: 3.6.3  
maven_installed_path: /opt  
maven_env_file: "/etc/profile.d/maven.sh"  

Dependencies
------------

Java is mandatory to install maven 

Example Playbook
----------------

create role:- ansible galaxy init anisble_role_linux_install_maven  
define role in playbook:-  
  
---
- name: install apache maven  
  hosts: localhost  
  become: yes  
  roles:  
  - role: ansible_role_linux_install_maven  


License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
