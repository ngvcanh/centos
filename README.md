# centos

CentOS 7

## CAMP

Install Apache, MysQL, PHP for Centos

- Apache 2.4.6
- MySQL 5.5.65-MariaDB
- PHP 5.6 / 7.3
- PHPMyAdmim 4.4.15.10 (for current document)
- Firewall
- Swap

Upload `camp` file to `/bin/` folder.

Chmod execute permission for `camp`:

```sh
chmod +x /bin/camp
```

Install service for server:

```sh
camp <php-version> <mysql-password> <swap-size>
```

- `<php-version>`: 7: 7.3; any: 5.6
- `<mysql-password>`: Set new password for mysql
- `<swap-size>`: Ex: 2048 - 2GB

```sh
camp 7 abc123passmysql 2048
```

## CVH

Create virtual host for apache

Virtual host file created on `/etc/httpd/sites-enabled/` folder.

Upload `cvh` file to `/bin/` folder.

Chmod execute permission for `camp`:

```sh
chmod +x /bin/cvh
```

Create host

```sh
cvh <domain> <document-root>
```

EX:

```sh
cvh mysite.com /var/www/mysite.com
```