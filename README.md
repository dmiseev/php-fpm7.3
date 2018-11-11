## PHP-FPM Image

[![Build Status](https://travis-ci.com/dmiseev/php-fpm7.3.svg?branch=master)](https://travis-ci.com/dmiseev/php-fpm7.3)

 **Helpful PHP-FPM image from official ubuntu:xenial**
 
 >
 > PHP-FPM version - 7.3
 >
 > DateTime - Europe/Kiev
 >
 > Supervisor installed globally
 >
 > Composer installed globally

## Tags
 * dmiseev/php-fpm7.3:stable

### Extensions:

 * php7.3-pgsql
 * php7.3-mysql
 * php7.3-opcache
 * php7.3-common
 * php7.3-mbstring
 * php7.3-mcrypt
 * php7.3-soap
 * php7.3-cli
 * php7.3-intl
 * php7.3-json
 * php7.3-xsl
 * php7.3-imap
 * php7.3-ldap
 * php7.3-curl
 * php7.3-gd
 * php7.3-dev
 * php7.3-fpm
 * php7.3-redis
 * php7.3-memcached
 * php7.3-mongodb
 * php7.3-bcmath
 * php7.3-imagick (`new`)
 * php7.3-zip (`new`)
 * php7.3-zmq (`new`)
 * php7.3-apcu (`new`)

### In addition

 * Supervisor (installed globally)
 * Composer (installed globally)
 
### Docker Compose yml

```yaml
version: "2"
services:
 php-fpm:
   image: dmiseev/php-fpm7.3
   volumes:
    - .:/usr/local/src/app
   working_dir: /usr/local/src/app
   extra_hosts:
    - "app:127.0.0.1"
```