# ./nginx/Dockerfile
FROM nginx:latest

# Copy Nginx configuration file
COPY ./default.conf /etc/nginx/conf.d/default.conf

# Set permissions for Nginx
RUN mkdir -p /var/www/html/ && \
    chmod -R 755 /var/www/html/
