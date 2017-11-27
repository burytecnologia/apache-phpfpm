# Alpine with Apache2 and PHP-FPM7

This is a container based on Alpine OS, Apache2 and PHP-FPM7. There images are build on docker pull alpine working with most of the regular needed modules (apcu, opcache, php-redis, etc.) are built in and configured like suggested on php.net.

## What's in this repository?

    Alpine:3.6
    Apache:2.4
    PHP-FPM:7.1
    [Bury Tecnologia](http://www.bury.com.br)

## Usage

docker run --name bury-web -t -v bury_log:/var/log -v bury_php7:/etc/php7 -v bury_apache2:/etc/apache2 -v bury_www:/var/www -p 80:80 -p 443:443 -d burytecnologia/apache-phpfpm:latest

