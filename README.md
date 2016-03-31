Ansible PHP-FPM
==============

Install and configure PHP-FPM on Debian server.

Installation
------------

git submodule add git@github.com/boostmyshoporganization/ansible-php-fpm roles/php-fpm

```yaml
roles:
    - php-fpm
```

Configuration
-------------

```yaml
php_fpm:
  fpm:
    upload_max_filesize: 2M
  cli:
  version: 55
  modules:
    - php5-cli
    - php5-curl
    - php5-mysqlnd
```