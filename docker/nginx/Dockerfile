FROM nginx:1.14

# The next instruction copies the NGINX configuration file from your disk to the Docker image.
COPY docker/nginx/default.conf /etc/nginx/conf.d/default.conf

#The next two instructions copy the css and img directories from your local disk to the NGINX root directory /var/www/html/ in the Docker image.

COPY css /var/www/html/css
COPY img /var/www/html/img

# The next instruction runs the chown command to transfer ownership of all static files to the nginx user. The nginx user is part of the base image.

RUN chown -R nginx:nginx /var/www/html