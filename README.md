PHP role
========

Install PHP and related packages. Debian / Ubuntu only.

---

List of variables:

<table>
  <thead>
    <tr>
      <th>Variable</th>
      <th>Type</th>
      <th>Description</th>
      <th>Defaults</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>php_system_packages</td>
      <td>Array</td>
      <td>PHP system packages to install</td>
      <td>build-essential, php5, php5-curl, php5-dev, php-pear, libpcre3-dev</td>
    </tr>
      <td>php_pear_channels</td>
      <td>Array</td>
      <td>List of pear channels to add</td>
      <td>None</td>
    </tr>
    <tr>
      <td>php_pear_packages</td>
      <td>Array</td>
      <td>List of pear packages to install</td>
      <td>None</td>
    </tr>
    <tr>
      <td>php_pecl_packages</td>
      <td>Array</td>
      <td>List of pecl packages to install</td>
      <td>None</td>
    </tr>
  </tbody>
</table>

---

Examples:

```
php_system_packages:
  - build-essential
  - php5
  - php5-curl
  - php5-dev
  - php5-gd
  - php5-imagick
  - php5-memcache
  - php5-mysql
  - php5-xdebug
  - php5-xsl
  - php-pear
  - php-soap
  - libapache2-mod-php5
  - libpcre3-dev

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
  - --onlyreqdeps Console_ProgressBar-beta
  - Horde/Horde_Yaml-beta

php_pecl_packages:
  - apc
```

---
