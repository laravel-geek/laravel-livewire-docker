# docker/php/Dockerfile
FROM php:8.3-fpm

# Установка зависимостей для PostgreSQL
RUN apt-get update && apt-get install -y \
    libpq-dev \
    && docker-php-ext-install pdo pdo_pgsql

# Копирование конфигурации PHP, если есть
COPY php.ini /usr/local/etc/php/

WORKDIR /var/www/laravel