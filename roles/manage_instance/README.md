Role Name
=========

General purpose role to manage instances on different cloud platforms.  Supported platforms are:
- Amazon Web Services (AWS)
- Azure
- Google Cloud Platform (GCP)
- VMware vSphere

Requirements
------------

The collection for the platform(s) being used must be installed on the controller.  For example, to use this role with AWS you will need the amazon.aws collection installed. 

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

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

GPLv3

Author Information
------------------

Ansible (https://github.com/ansible)
