# Usar a imagem oficial do PHP 8.3 com Apache
FROM php:8.3-apache

# Instalar extensões necessárias do linux
RUN apt-get update && apt-get install -y \
    libpng-dev \
    libjpeg-dev \
    libfreetype6-dev \
    git 

# Instalar extensões do PHP
RUN docker-php-ext-install gd pdo pdo_mysql

# Instalar o Xdebug
RUN pecl install xdebug \
    && docker-php-ext-enable xdebug
  
# Configurações do Xdebug
COPY xdebug.ini /usr/local/etc/php/conf.d/xdebug.ini

# Ativar o mod_rewrite do Apache
RUN a2enmod rewrite

# Copiar os arquivos do projeto para o diretório padrão do Apache
COPY ../ /var/www/html/

# Configuração php.ini
COPY custom.ini /usr/local/etc/php/conf.d/custom.ini

# Permissão para o usuário alterar o Shell
RUN usermod -s /bin/bash www-data