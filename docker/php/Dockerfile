FROM php:8.0.10-fpm-alpine3.14

COPY --from=mlocati/php-extension-installer /usr/bin/install-php-extensions /usr/local/bin/

RUN install-php-extensions xdebug-stable @composer-2.1.8

WORKDIR /var/www/app
