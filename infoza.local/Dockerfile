FROM php:7.2-apache

# Устанавливаем необходимые расширения
RUN docker-php-ext-install mysqli pdo pdo_mysql

# Устанавливаем Xdebug версии 2.9.8
#RUN pecl install xdebug-2.9.8 \
#    && docker-php-ext-enable xdebug
RUN pecl install xdebug-3.0.1 && docker-php-ext-enable xdebug

# Включаем модуль mod_rewrite для Apache
RUN a2enmod rewrite

# Включаем модуль ssl для Apache
RUN a2enmod ssl