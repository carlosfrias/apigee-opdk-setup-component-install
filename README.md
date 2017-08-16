Apigee OPDK Setup Component
=========

This roles is used to setup individual Apigee OPDK components. 

Requirements
------------

The installation of Apigee OPDK requires root access. Credentials must also be supplied to override the empty placeholders
provided here. It is recommended that credentials be consolidated into a single credentials.yml file that can be stored 
separately. It is assumed that files containing credentials are stored in the ~/.apigee folder. 

Role Variables
--------------

Variable defaults are managed in the role apigee-opdk-setup-default-settings:

Path to the Apigee setup script

     apigee_setup: 
     
Name of the installation profile to invoke

     profile: '' 
     
Path to the silent installation file
     
     opdk_installation_config_file: ''
     
Version of OPDK to install
     
     opdk_version: '4.16.09'
     
Email of the Apigee user
     
     opdk_user_email: ''
     
Password of the Apigee user
     
     opdk_user_pass: ''
     
     

Dependencies
------------

This role depends on the following roles:

* apigee-opdk-setup-default-settings


Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

Apache

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
