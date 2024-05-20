# ./nginx/Dockerfile
FROM nginx:latest

# Copy Nginx configuration file
COPY ./default.conf /etc/nginx/conf.d/default.conf

# Set permissions for Nginx
RUN chmod -R 755 /var/www/html/
