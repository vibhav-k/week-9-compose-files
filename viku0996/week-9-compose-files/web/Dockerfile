
FROM ubuntu
USER root

RUN apt-get -y update && \
  apt-get install -y nginx php php-mysql && \
  rm -rf /var/lib/apt/lists/* && \
  echo "\ndaemon off;" >> /etc/nginx/nginx.conf && \
  chown -R www-data:www-data /var/lib/nginx

WORKDIR /etc/nginx
ADD ./web/html /var/www/html
ADD ./data/files/default sites-enabled/default
EXPOSE 80

#CMD ["nginx"]
#ENTRYPOINT ["/usr/sbin/nginx"]

