code-server
=========

code-server is VS Code running on a remote server, accessible through the browser. This role installs code-server and runs it as a systemd service.

Requirements
------------

None

Role Variables
--------------

code_server_directory: Directory in which visual studio code will run.
code_server_password: Password to login 

Dependencies
------------

None

Example Playbook
----------------

Visual Studio Code will be available under https://[your-ip]:8443

    - hosts: servers
      vars:
        code_server_directory: ~/my_app_dir
        code_server_password: myPassword
      roles:
         - code-server

License
-------

BSD

Author Information
------------------

This role was createdin 2019 by Patrick Schubert <Patrick.Schubert@atos.net>
