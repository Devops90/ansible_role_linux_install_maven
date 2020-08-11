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

pass variables as extravariables at run time:-  
  
ansible-playbook maven.yml -i /inventory  
ansible-playbook maven.yml -i /inventory -e "maven_major=3 maven_version=3.6.3 maven_installed_path= /opt maven_env_file=/etc/profile.d/maven.sh" 
  
  

pass variables in playbook:-  
  
---
- name: install apache maven  
  hosts: localhost  
  become: yes  
  roles:
  - role: ansible_role_linux_install_maveni  
    maven_major: 3  
    maven_version: 3.6.3  
    maven_installed_path: /opt  
    maven_env_file: /etc/profile.d/maven.sh  


License
-------

BSD

Author Information
------------------

Auther: Haribabu Challa  
malid: challaharibabu70@gmail.com  

