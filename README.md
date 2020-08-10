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

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
