# Base image
FROM nginx:latest

# Copy the static website content
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy the Nginx configuration
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
