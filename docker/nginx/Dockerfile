FROM nginx:1.23.3-alpine
COPY ./docker/nginx/nginx.conf /etc/nginx/nginx.conf
COPY ./docker/nginx/fastcgi.conf /etc/nginx/fastcgi.conf
COPY ./docker/nginx/conf.d/local.conf /etc/nginx/conf.d/default.conf
COPY ./src/public /var/www/html/public
