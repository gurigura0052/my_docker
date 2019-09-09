ARG PHP_VERSION

FROM php:${PHP_VERSION}-apache

# WordPressに必要な拡張モジュール
RUN apt-get update && apt-get install -y \
libmagickwand-dev libssh2-1-dev libmcrypt-dev libxml2-dev \
&& pecl install imagick mcrypt-1.0.2 ssh2-1.1.2 \
&& docker-php-ext-enable imagick mcrypt ssh2 \
&& docker-php-ext-install exif mysqli sockets xml zip gd
