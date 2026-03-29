# Use official PHP + Apache image
FROM php:8.2-apache

# Enable Apache mod_rewrite (optional but common)
RUN a2enmod rewrite

# Install PHP extensions (add/remove based on your needs)
RUN docker-php-ext-install mysqli pdo pdo_mysql

# Copy project files into Apache document root
COPY . /var/www/html/

# Set correct permissions
RUN chown -R www-data:www-data /var/www/html

# Expose port 80
EXPOSE 80

# Apache starts automatically via base image
