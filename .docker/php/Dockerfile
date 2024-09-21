# Use a imagem oficial do PHP
FROM php:8.1-apache

# Instalar extensões necessárias
RUN apt-get update && apt-get install -y \
    curl \
    unzip \
    && docker-php-ext-install pdo pdo_mysql \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# Instalar o Composer
COPY --from=composer:latest /usr/bin/composer /usr/local/bin/composer

# Seta o arquivo de trabalho 
WORKDIR /var/www

# Copia o php.ini personalizado
COPY php.ini /usr/local/etc/php/

# Configurar permissões
RUN chown -R www-data:www-data /var/www
