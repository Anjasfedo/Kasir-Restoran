# Use the official PHP 8.1 FPM image
FROM php:8.1-fpm

# Specify the desired user ID
ARG USER_ID=1001

# Install necessary PHP extensions
RUN docker-php-ext-install mysqli pdo pdo_mysql gd

# Set the working directory
WORKDIR /var/www/html/

# Ensure proper permissions for the uploads directory
RUN mkdir -p /var/www/html/src/img && \
    chown -R ${USER_ID}:www-data /var/www/html/src/img && \
    chmod -R 755 /var/www/html/src/img

# Set the desired user ID as the user for running PHP
USER ${USER_ID}
