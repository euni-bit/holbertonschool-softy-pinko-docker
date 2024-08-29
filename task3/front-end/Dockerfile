# Use the latest Nginx image as the base image
FROM nginx:latest

# Copy the front-end files to the appropriate directory in the Docker image
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy the custom Nginx configuration file to the Docker image
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
