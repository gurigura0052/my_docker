ARG PHP_VERSION

FROM php:${PHP_VERSION}-apache

# WordPressに必要な拡張モジュール
RUN apt-get update && apt-get install -y \
libfreetype6-dev \
libjpeg62-turbo-dev \
libpng-dev \
libxml2-dev \
&& docker-php-ext-install mysqli gd mbstring opcache xml
