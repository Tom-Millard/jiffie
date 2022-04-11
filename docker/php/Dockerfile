FROM composer:2 as composer
FROM php:8.1.0-fpm as php

RUN apt-get update
RUN apt-get install -y git zip unzip curl

RUN pecl install xdebug-3.1.4 && docker-php-ext-enable xdebug

COPY --from=composer /usr/bin/composer /usr/bin/composer

RUN apt-get clean
