Role Name
=========

NTP server is a server for synchronizing time between the infrastructure.

Requirements
------------

- Ansible control server
- Ubuntu

Role Variables
--------------

You can override those variable(s) in your playbook

ntp_server1
ntp_server2   
ntp_server3
ntp_server4
ntp_timezone

Example Playbook
----------------

    - hosts: ntp
      
      vars: 
        ntp_server1: 0.pool.ntp.org
        ntp_server2: 1.pool.ntp.org
        ntp_server3: 2.pool.ntp.org 
        ntp_server4: 3.pool.ntp.org
        ntp_timezone: Europe/Amsterdam

      roles: 
        - ansible-role-ntp-server

License
-------

GNU GPLv3


Author Information
------------------ 

www.bitfinity.nl
