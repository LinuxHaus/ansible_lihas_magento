Role Name
=========

lihas_magento

Requirements
------------

'python-pymysql' has to be installed on mysql server

Role Variables
--------------

Enable DNS Settings on UCS-Servers with 'dns.type' = 'ucs', might become a seperate role

needs ssh-access tu UCS server

```
dns.type: ucs
dns.host: hostname-in-zone
dns.zone: zone-in-dns-server
dns.ip: ip-of-host
dns.ucs_server: name-of-ucs-server
roles.magento.hostname:
roles.magento.db_host:
roles.magento.db_user:
roles.magento.db_pass:
roles.magento.db_name:
roles.magento.user: filesystem user
roles.magento.version: e.g. 2.3.6
roles.magento.repo_user: repo.magento.com user
roles.magento.repo_pass:
```

Dependencies
------------

* lihas_apache

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: magento
      roles:
         - lihas_magento

License
-------

GPL-3.0-or-later

Author Information
------------------

Adrian Reyer <lihas@lihas.de>
