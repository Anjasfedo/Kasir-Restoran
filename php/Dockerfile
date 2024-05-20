FROM php:8.1-fpm

# Install necessary PHP extensions
RUN docker-php-ext-install mysqli pdo pdo_mysql gd

# Set the working directory
WORKDIR /var/www/html/

# Ensure proper permissions for the uploads directory
RUN mkdir -p /var/www/html/uploads && \
    chown -R www-data:www-data /var/www/html/uploads && \
    chmod -R 755 /var/www/html/uploads