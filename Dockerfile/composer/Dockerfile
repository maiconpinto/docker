FROM composer

FROM php:7-apache

COPY --from=composer /usr/bin/composer /usr/bin/composer

RUN apt-get update && apt-get install -y \
    libicu-dev \
    zip \
    unzip

RUN docker-php-ext-install intl

WORKDIR /app

ENTRYPOINT [ "composer" ]