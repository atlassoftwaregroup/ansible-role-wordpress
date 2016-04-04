wordpress
=========
Adds nginx configs for wordpress in /etc/nginx/global/

Requirements
------------
  - nginx
  - wordpress 

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------
None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: jnakatsui.wordpress }

License
-------
The source code is licensed under GPL v3.

Note
----
Commented out the following from wordpress.conf

# Directives to send expires headers and turn off 404 error logging.
# location ~* \.(js|css|png|jpg|jpeg|gif|ico)$ {
#         expires 24h;
#         log_not_found off;
#         try_files $uri $uri/ /index.php?$args;
# }
