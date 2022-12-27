FROM php:8.2.1RC1-fpm-alpine3.17

COPY ./src /var/www/html
WORKDIR /var/www/html
VOLUME /var/www/html

# Install composer
RUN curl -sS https://getcomposer.org/installer \
    | php -- --install-dir=/usr/bin --filename=composer --version=2.5.1

# Install composer packages
RUN php /usr/bin/composer install --no-dev -d /var/www/html
