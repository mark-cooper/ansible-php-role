PHP role
========

[![Build Status](https://travis-ci.org/mark-cooper/ansible-php-role.png?branch=master)](https://travis-ci.org/mark-cooper/ansible-php-role)

Install PHP and related packages. Debian / Ubuntu only.

**Core packages:**

- build-essential
- php5
- php5-dev
- php-pear
- libpcre3-dev

---

List of variables:

```yml
# PHP system packages to install
php_system_packages: []
# List of pear channels to add
php_pear_channels: []
# List of pear packages to install
php_pear_packages: []
# List of pecl packages to install
php_pecl_packages: []

```

---

Examples:

```
php_system_packages:
  - php5-curl
  - php5-gd
  - php5-imagick
  - php5-memcache
  - php5-mysql
  - php5-xdebug
  - php5-xsl
  - php-soap
  - libapache2-mod-php5

php_pear_channels:
  - pear.horde.org

php_pear_packages:
  - --onlyreqdeps Auth_SASL
  - --onlyreqdeps DB
  - --onlyreqdeps DB_DataObject
  - --onlyreqdeps Structures_DataGrid-beta
  - --onlyreqdeps Structures_DataGrid_DataSource_DataObject-beta
  - --onlyreqdeps Structures_DataGrid_DataSource_Array-beta
  - --onlyreqdeps Structures_DataGrid_Renderer_HTMLTable-beta
  - --onlyreqdeps HTTP_Client
  - --onlyreqdeps HTTP_Request
  - --onlyreqdeps Log
  - --onlyreqdeps Mail
  - --onlyreqdeps Mail_Mime
  - --onlyreqdeps Net_SMTP
  - --onlyreqdeps Pager
  - --onlyreqdeps XML_Serializer-beta
  - Horde/Horde_Yaml-beta

php_pecl_packages:
  - apc
```

---
