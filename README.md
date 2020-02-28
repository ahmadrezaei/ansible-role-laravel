Role Name
=========

Installs and configures latest version of laravel.

Requirements
------------

No special requirements.

Role Variables
--------------

```yaml
project_url: example.com
create_database: false
database_name: laravel
database_username: laravel
database_password: secret
use_redis: true
schedule: true
```

Dependencies
------------

- geerlingguy.git
- kbrebanov.zip
- kbrebanov.unzip
- geerlingguy.composer
- geerlingguy.mysql
- robertdebock.redis
- geerlingguy.nginx
- geerlingguy.repo-remi
- geerlingguy.php
- geerlingguy.php-versions
- geerlingguy.php-redis
- geerlingguy.php-mysql
- geerlingguy.php-pecl
- geerlingguy.pip
- geerlingguy.supervisor
- geerlingguy.certbot


Example Playbook
----------------


    - hosts: all
      roles:
        - role: ahmadrezaei.laravel
          project_url: example.com
          create_database: true
          enable_ssl: true

License
-------

MIT / BSD