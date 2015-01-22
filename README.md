Superadmin
==========

Create a superadmin user:

- authenticated with ssh-key, 
- can use sudo without password.

Warning
-------

This role is dangerous because the superadmin user will have free sudo access !
Running a program with the superadmin user has the same security implications
as using the root user. Only use if you know what you're doing: do **not**
expose users created with this role to internet. It is solely for
administration purposes.

Requirements
------------

You must know the name of the user you want created.

Role Variables
--------------

User is the username.

Example Playbook
----------------

Example usage:

    - hosts: servers
      roles:
         - { role: username.rolename, user: james }

License
-------

BSD
