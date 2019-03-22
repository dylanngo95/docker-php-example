FROM ubuntu:18.04

MAINTAINER "Tinh Ngo"

RUN apt-get update \ 
    && apt-get install -y nginx \
    && apt-get install -y php7.2 php7.2-fpm


WORKDIR /var/www

CMD ["/bin/bash", "-c", "/usr/sbin/service php7.2-fpm start && nginx -g 'daemon off;'"]