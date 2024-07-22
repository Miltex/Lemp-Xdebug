FROM php:8.3-fpm

RUN apt-get update && apt-get install -y zlib1g-dev && apt-get install -y libpng-dev  && apt-get install -y libzip-dev  

RUN pecl install xdebug-3.3.2 && docker-php-ext-enable xdebug
RUN docker-php-ext-install mysqli
RUN docker-php-ext-install gd
RUN docker-php-ext-install zip

COPY --from=composer /usr/bin/composer /usr/bin/composer

RUN curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
RUN . ~/.nvm/nvm.sh && nvm install node

RUN usermod -u 1000 www-data