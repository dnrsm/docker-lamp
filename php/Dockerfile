FROM php:7.2-apache
RUN apt-get update \
  && apt-get install -y libfreetype6-dev libjpeg62-turbo-dev libpng-dev libmcrypt-dev \
  && docker-php-ext-install pdo_mysql mysqli mbstring gd iconv \
  && pecl install xdebug \
  && a2enmod rewrite
COPY php.ini /usr/local/etc/php/