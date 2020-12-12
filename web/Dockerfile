FROM php:7.2-apache

COPY ../file-web /var/www/html/
# WORKDIR /var/www/html/
# CMD [ "php", "./your-script.php" ]
RUN docker-php-extinstall pdo pdo_mysql

HEALTHCHECK CMD curl --fail http://localhost || exit 0 
