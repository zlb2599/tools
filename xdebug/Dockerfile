FROM php:5.6-fpm

RUN cp /usr/local/etc/php/php.ini-development /usr/local/etc/php/php.ini
RUN echo 'date.timezone = PRC'>>/usr/local/etc/php/php.ini
RUN echo 'xdebug.idekey=PHPSTORM'>>/usr/local/etc/php/php.ini
RUN echo 'xdebug.remote_host=host.docker.internal'>>/usr/local/etc/php/php.ini
RUN echo 'xdebug.remote_port=9001'>>/usr/local/etc/php/php.ini
RUN echo 'xdebug.remote_enable=1'>>/usr/local/etc/php/php.ini
RUN echo 'user = www-data'>>/usr/local/etc/php-fpm.d/www.conf
RUN echo 'group = www-data'>>/usr/local/etc/php-fpm.d/www.conf
RUN pecl channel-update pecl.php.net
RUN pecl install https://pecl.php.net/get/xdebug-2.5.5.tgz
RUN docker-php-ext-enable xdebug

WORKDIR /var/www/html/
