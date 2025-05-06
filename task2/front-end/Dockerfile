FROM nginx:latest

COPY . /var/www/html/softy-pinko-front-end

COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

RUN chmod -R 755 /var/www/html/softy-pinko-front-end
