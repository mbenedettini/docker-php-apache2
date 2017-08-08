# Apache2+PHP7 Docker image

Includes PDO Mysql, see the [Dockerfile](https://github.com/mbenedettini/docker-php-apache2/blob/master/Dockerfile) for more details.

You should mount:

1. A php.ini file in /usr/local/etc/php/php.ini. I'm using the one provided by the official php repo and it's working pretty well: https://github.com/php/php-src/blob/master/php.ini-production.
2. Your site in /var/www/html
3. A different Apache config in /etc/apache2/sites-available/000-default.conf if the one provided does not suit you. Here's the one I'm currently using https://gist.github.com/mbenedettini/361a75ebc448d4ec619880ef4f779fab
