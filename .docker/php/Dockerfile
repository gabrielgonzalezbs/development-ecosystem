# Use a imagem oficial do PHP
FROM php:8.1-apache

# Instalar extensões necessárias
RUN docker-php-ext-install pdo pdo_mysql

# Seta o arquivo de trabalho 
WORKDIR /var/www

# Copia o php.ini personalizado
COPY php.ini /usr/local/etc/php/

# Configurar permissões
RUN chown -R www-data:www-data /var/www
