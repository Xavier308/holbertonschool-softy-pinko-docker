# Use Nginx latest image as the base
FROM nginx:latest

# Copy the front-end files to the Nginx server directory
COPY softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy the Nginx configuration file
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
