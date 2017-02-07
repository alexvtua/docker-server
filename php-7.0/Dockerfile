FROM php:7.0

RUN apt-get update

RUN pecl install xdebug -yqq

COPY ./xdebug.ini /etc/php7.0/mods-availible/xdebug.ini

RUN rm -rf /var/lib/apt/lists/*

RUN ln -sf /dev/stderr /var/log/fpm-php.www.log

VOLUME /var/www

EXPOSE 9000
