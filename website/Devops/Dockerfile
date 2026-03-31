# -----------Stage1--------------

FROM php:8.2-apache

WORKDIR /app

COPY /website /var/www/html/

RUN a2enmod rewrite

#RUN docker-php-ext-install mysqli

RUN chown -R www-data:www-data /var/www/html
#CMD ["php", "-S", "0.0.0.0:8000", "index.php"]

EXPOSE 80
